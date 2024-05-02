<script setup lang="ts">
import ContactForm from './ContactForm.vue';
import More from './More.vue';
</script>

<template>
  <div class="bg-indigo-600 px-4 py-3 text-white">
    <p class="text-center md:text-2xl text-sm font-medium uppercase">
      Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </p>
  </div>
  <div
    class="bg-[url('/img-bg-section.jpg')] bg-cover bg-center bg-no-repeat w-full"
  >
    <div class="flex flex-col md:flex-row justify-center items-center">
      <div>
        <ContactForm />
      </div>
      <div>
        <img src="/profile.webp" alt="photo profile" />
      </div>
    </div>
  </div>
  <div>
    <More />
  </div>
  <div
    class="bg-[url('/banner.webp')] bg-cover bg-center bg-no-repeat w-full flex justify-center p-8"
  >
    <div class="text-center text-white my-4">
      <p class="text-xl">Texto:</p>
      <p class="py-4 text-2xl">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero nesciunt
        velit quos? <span class="text-[#11C6DD]">Tempora delectus</span>
      </p>
      <p class="text-2xl">Lorem ipsum dolor sit amet consectetur</p>
      <button
        type="button"
        class="mt-8 py-4 px-10 text-2xl bg-[#11C6DD] rounded-2xl border-[#11C6DD] border-2 border-solid hover:border-white"
      >
        Garanta sua vaga
      </button>
    </div>
  </div>

  <div class="flex flex-col lg:flex-row justify-center items-center lg:items-start  my-16">
    <div class="lg:block flex flex-col">
      <img src="/profile1.webp" alt="Phot Profile" />
      <p class="text-center text-lg font-semibold p-4">Texto Texto Texto</p>
      <div>
        <img src="/tes.webp" alt="" />
      </div>
    </div>

    <div class="lg:max-w-[35%] max-w-[90%] text-justify md:text-xl text-sm mt-8 md:mt-10">
      <div class="flex flex-col">
        <div>
          <span class="text-xl font-bold block text-[#11C6DD]">Marcus Solon</span>
          <span class="text-lg">Treinador</span>
        </div>
        <p class="my-2">
          Eu sou o Marcus Solon. Ao longo de minha carreira como Engenheiro Civil e Terapeuta Familiar Sistêmico, tenho ajudado famílias a restaurarem seus laços e encontrarem equilíbrio emocional.
        </p>
        <p class="my-2">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio id
          distinctio magni doloremque assumenda blanditiis, asperiores fugit
          laboriosam sapiente eum aliquam repellendus modi, provident quia, at
          officia ipsum autem facilis!
        </p>
        <p class="my-2">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio id
          distinctio magni doloremque assumenda blanditiis, asperiores fugit
          laboriosam sapiente eum aliquam repellendus modi, provident quia, at
          officia ipsum autem facilis!
        </p>
        <p class="my-2">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio id
          distinctio magni doloremque assumenda blanditiis, asperiores fugit
          laboriosam sapiente eum aliquam repellendus modi, provident quia, at
          officia ipsum autem facilis!
        </p>
      </div>
    </div>
  </div>

  <!-- Footer -->
  <div class="bg-[#000000] text-white ">
    <div class="p-8 flex justify-evenly items-center">
      <p class="text-xl ">APORTEFAC</p>
      <p class="text-sm">2024 © Todos os Direitos Reservados</p>
    </div>
  </div>
</template>
