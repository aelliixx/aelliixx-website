<script setup lang="ts">
defineProps(["title", "imageUrl", "link", "tech"]);
</script>

<template>
  <div class="card">
    <img v-if="imageUrl" :src="imageUrl" alt="" />
    <div class="content">
      <h3 v-if="!link" class="title">{{ title }}</h3>
      <a v-else :href="link" class="title">{{ title }}</a>
      <div class="body">
        <slot />
      </div>
      <p class="tech" v-if="tech">Tech:<br />{{ tech }}</p>
    </div>
  </div>
</template>

<style scoped lang="scss">
.card {
  display: flex;
  flex-direction: column;
  background-color: var(--clr-bg-900);
  border-radius: 10px;
  transition: box-shadow 300ms ease-in-out;
  overflow: hidden;

  grid-column: span 2;
  grid-row: span 2;

  img {
    object-fit: cover;
  }

  .content {
    display: flex;
    flex-direction: column;
    height: 100%;
    padding: 1rem;
  }

  .title {
    font-size: 1.5rem;

    &:is(a):is(:hover, :focus-visible) {
      text-decoration: underline;
    }
  }

  .body {
    line-height: 1.3;
    margin-block-end: 1rem;
  }

  .tech {
    margin-block-start: auto;
    font-size: 0.8em;
  }

  &:is(:hover) {
    box-shadow: 0 0 2rem var(--clr-accent-200);
  }
}
</style>
