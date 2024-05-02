<script setup lang="ts">
import { ref } from 'vue';
import InputPhoneNumber from './InputPhoneNumber.vue';

const email = ref<string>('');
const phone = ref<string>('');

const emailError = ref<boolean>(false);
const phoneError = ref<boolean>(false);

const checkForm = (e: Event) => {
  e.preventDefault();

  if (!email.value) {
    console.log('entrei');
     emailError.value = true;
  }

}

</script>

<template>
  <!--
      Heads up! 👋
    
      Plugins:
        - @tailwindcss/forms
    -->

  <div class="w-full mx-auto max-w-screen-xl px-4 py-16 sm:px-6 lg:px-8">
    <div class="mx-auto max-w-lg md:max-w-none text-center lg:max-w-lg text-white">
      <h1 class="font-bold text-3xl">Get started today!</h1>

      <p class="mt-4 text-2xl font-medium ">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Et libero nulla
        eaque error neque ipsa culpa autem, at itaque nostrum!
      </p>
    </div>

    <form action="#" @submit.prevent="checkForm" class="mx-auto mb-0 mt-8 max-w-md md:max-w-none lg:max-w-md space-y-4">
      <div>
        <label for="email" class="sr-only">Email</label>

        <div class="relative">
          <input
            type="email"
            class="w-full rounded-lg p-4 pe-12 text-sm shadow-sm border-2"
            placeholder="Enter email"
            name="email"
            required
            v-model="email"
          />

          <p v-if="emailError != false" class="text-red-900 font-bold text-lg">*Email invalido</p>

          <span class="absolute inset-y-0 end-0 grid place-content-center px-4">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="size-4 text-gray-400"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M16 12a4 4 0 10-8 0 4 4 0 008 0zm0 0v1.5a2.5 2.5 0 005 0V12a9 9 0 10-9 9m4.5-1.206a8.959 8.959 0 01-4.5 1.207"
              />
            </svg>
          </span>
        </div>
      </div>

      <div>
        <div class="relative">
          <InputPhoneNumber />
        </div>
      </div>

      <div class="flex w-full gap-4 text-white text-lg font-semibold">
        <span><i class="fa-regular fa-calendar"></i> DATA: 12/12/2012</span>
        <span><i class="fa-regular fa-clock"></i> HORA: 00:00</span>
      </div>

      <div class="flex items-center justify-between w-full">
        <button
          type="submit"
          class="inline-block rounded-lg bg-blue-500 px-5 py-3 text-lg font-medium text-white w-full border-2 border-solid border-blue-500 hover:border-white"
        >
          Garantir Minha Vaga Agora
        </button>
      </div>
    </form>
  </div>
</template>
