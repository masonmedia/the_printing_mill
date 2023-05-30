<script setup>
import { RouterView } from 'vue-router'
import Nav from './components/TheNav.vue'

</script>

<template>
  <div class="page-fade" style="overflow-x: hidden;">
    <header>
      <Nav></Nav>
    </header>

    <RouterView />
  </div>
</template>

<style scoped>
nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}
</style>
