<script setup>
import ExperienceCard from "./ExperienceCard.vue";
defineProps(['experiences']);
</script>

<template>
  <ul>
    <ExperienceCard v-for="(item, index) in experiences" :key="index" :experience="item" />
  </ul>
</template>