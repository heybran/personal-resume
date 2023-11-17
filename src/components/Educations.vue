<script setup>
import EducationCard from "./EducationCard.vue";
defineProps(['educations']);
</script>

<template>
  <ul>
    <EducationCard v-for="(item, index) in educations" :key="index" :education="item" />
  </ul>
</template>