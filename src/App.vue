<template>
    <div class="fixed top-0 left-0">
      <h1>Menu</h1>
      <ul>
        <li>Good morning</li>
        <li>Bom dia</li>
        <li>Bongiorno</li>
        <li>Buenos dias</li>
        <li>Bonjour</li>
      </ul>
    </div>
    <div class="fixed z-10 top-0 left-0 bg-green-300 w-full h-12 text-left transition-all ease-in-out" 
    :class="{'translate-x-0': !menuOpen, 'translate-x-3/4': menuOpen}">
        <button @click="menuOpen = !menuOpen">Open/Close</button>
        Fxed scroll header
    </div>
    <div class="absolute top-12 left-0 bg-slate-500 w-full min-h-screen text-left transition-all ease-in-out" 
    :class="{'translate-x-0': !menuOpen, 'translate-x-3/4': menuOpen}">
      <div> {{ new Array(500).fill('Lorem ipsum').join(' ') }}</div>
    </div>
  
 
</template>

<script setup lang="ts">
import { ref } from 'vue';

const menuOpen = ref(false)
</script>
<style scoped>
body {
  overflow-x: hidden;
}
</style>
