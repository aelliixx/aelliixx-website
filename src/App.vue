<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
import Navbar from "./components/Navbar.vue";
</script>

<template>
  <Navbar />
  <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg" class="noise">
    <filter id="noiseFilter">
      <feTurbulence type="fractalNoise" baseFrequency="0.65" numOctaves="3" stitchTiles="stitch" />
    </filter>
  </svg>
  <RouterView />
</template>

<style scoped></style>
