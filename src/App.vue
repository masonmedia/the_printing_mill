<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Nav from './components/TheNav.vue'
</script>

<template>
  <header>
    <Nav></Nav>
  </header>

  <RouterView />
</template>

<style scoped>
nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}
</style>
