<template>
  <div class="absolute top-0 left-0 z-0">
    <h1>Menu</h1>
    <ul>
      <li>Good morning</li>
      <li>Bom dia</li>
      <li>Bongiorno</li>
      <li>Buenos dias</li>
      <li>Bonjour</li>
    </ul>
  </div>
  <div class="absolute top-0 z-0 bg-slate-500 w-full h-screen text-left transition-all ease-in-out" :class="{'left-0': !menuOpen, 'left-3/4': menuOpen}">
    <button @click="menuOpen = !menuOpen">Switch collapse</button>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const menuOpen = ref(false)
</script>
<style scoped></style>
