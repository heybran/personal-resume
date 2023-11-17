<script setup>
import HighlightCard from './HighlightCard.vue';
defineProps(['highlights']);
</script>

<template>
  <ul keep-list-style>
    <HighlightCard v-for="(item, index) in highlights" :key="index" :highlight="item" />
  </ul>
</template>