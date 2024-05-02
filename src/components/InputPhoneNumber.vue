<script setup lang="ts">
 import { ref, defineProps, defineEmits } from 'vue';
 const phone = ref(null);

 const { emit } = defineEmits();

 const incrementCounter = () => {
    
 }

</script>

<template>
<vue-tel-input 
    v-model="phone" 
    mode="international" 
    placeholder=""
    required
    style=""
    >
</vue-tel-input>
</template>



