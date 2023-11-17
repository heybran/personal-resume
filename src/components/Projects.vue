<script setup>
import ProjectCard from "./ProjectCard.vue";
defineProps(['projects']);
</script>

<template>
  <ul>
    <ProjectCard v-for="(item, index) in projects" :key="index" :project="item" />
  </ul>
</template>