<script setup lang="ts">
defineProps(["name", "imageUrl", "source"]);
</script>

<template>
  <div class="card">
    <img v-if="imageUrl" :src="imageUrl" class="image" :alt="name" />
    <div class="content">
      <h3 class="name">{{ name }}</h3>
      <p class="tech" v-if="source">{{ source }}</p>
      <div class="body">
        <slot />
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">

.card {
  display: flex;
  flex-direction: row;
  align-items: start;
  background-color: var(--clr-bg-900);
  border-radius: 10px;
  transition: box-shadow 300ms ease-in-out;
  overflow: hidden;

  grid-column: span 2;
  grid-row: span 2;



  .image {
    margin: 1rem;
    aspect-ratio: 1 / 1;
    border-radius: 200rem;
  }

  img {
    object-fit: contain;
  }

  .content {
    display: flex;
    flex-direction: column;
    height: 100%;
    padding: 1rem;
  }

  .name {
    font-size: 1.5rem;

    &:is(a):is(:hover, :focus-visible) {
      text-decoration: underline;
    }
  }

  .body {
    line-height: 1.3;
    margin-block-start: 0.5rem;
  }

  .tech {
    font-size: 0.8em;
  }

  &:is(:hover) {
    box-shadow: 0 0 2rem var(--clr-accent-200);
  }
}

@media (max-width: 425px) {
  .card {
    flex-direction: column;

    .content {
      padding-block-start: 0;
    }
    .image {
      align-self: center;
    }
  }
}
</style>
