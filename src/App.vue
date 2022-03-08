<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <div class="flex flex-col h-screen">
    <header class="max-w-full md:max-w-7xl mx-auto">
      <nav class="m-2">
        <RouterLink class="md:text-lg m-2" to="/">Home</RouterLink>
        <RouterLink class="md:text-lg m-2" to="/about">About</RouterLink>
        <RouterLink class="md:text-lg m-2" to="/projects">Projects</RouterLink>
      </nav>
    </header>
    <div class="flex-1 overflow-y-auto">
      <RouterView />
    </div>
  </div>
</template>

<style>
@import "@/assets/base.css";

#app {
  height: 100vh;
  width: 100vw;
}
</style>
