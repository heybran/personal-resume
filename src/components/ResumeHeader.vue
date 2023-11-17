<script setup>
import Contact from "./Contact.vue";
defineProps(['name', 'description', 'authorImage']);
</script>

<template>
  <div class="wrapper">
    <div class="right-column">
      <h1>{{ name }}</h1>
      <small>Web Developer</small>
      <p class="description">{{ description }}</p>
      <Contact />
    </div>
    <div class="left-column">
      <img :src="authorImage" alt="Image of the author" style="max-width: 100%; border-radius: 1rem;" width="160" height="160"/>
    </div>
  </div>
</template>

<style scoped>
.wrapper {
  display: grid;
  padding-block: 3rem; 
  gap: 0.5rem; 
  grid-template-columns: 250px 1fr;
  & > .left-column {
    grid-column: 1 / 2;
    grid-row: 1 / 2;
  }
  & h1 {
    margin-block: 0;
    font-weight: 700;
  }
  & small {
    margin-top: -0.5rem;
    display: block;
  }
}
</style>