<script setup lang="ts"></script>

<template>
  <header class="navbar">
    <a href="/" class="logo link">aelliixx.</a>
    <nav class="links">
      <a class="link" href="#experience">experience.</a>
      <a class="link" href="#projects">projects.</a>
      <a class="link" href="#work">work.</a>
      <a class="link" href="#contact">contact.</a>
    </nav>
  </header>
</template>

<style scoped>
.navbar {
  display: flex;
  align-items: center;
  padding-block: 0.75rem;
}

.logo {
  font-size: 1.75rem;
}

.links {
  margin-inline-start: auto;
  display: flex;
  gap: 3rem;
  font-size: 1.25rem;
}
</style>
