<script setup>
defineProps(['experience']);
</script>

<template>
  <li>
    <h3>
      {{ experience.role }} {{ experience.company ? "- " + experience.company : '' }}
    </h3>
    <small>{{ experience.time }}</small>
    <p v-html="experience.description"></p>
  </li>
</template>
