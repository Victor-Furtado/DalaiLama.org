<script setup lang="ts">
import frases from './data.json';

const frase = frases[Math.floor(Math.random() * frases.length)];

</script>

<template>
  <div class="w-screen h-screen bg-gradient-to-tr from-gray-700 to-black flex items-center justify-between">
    <img src="/dalai-lama.png" alt="Dalai Lama" class="h-full pt-5 pl-16">
    <div class="w-full">
      <div class="mx-auto rounded-lg text-white h-52 w-96 space-y-1">
        <p class="text-right text-3xl text">"{{ frase }}"</p>
        <h1 class="text-right text-sm">Dalai Lama, 2022</h1>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Satisfy&display=swap');

.text {
  font-family: 'Satisfy', cursive;
}

img {
  -webkit-filter: grayscale(100%);
  filter: grayscale(100%);
}
</style>