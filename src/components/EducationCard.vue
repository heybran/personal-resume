<script setup>
defineProps(['education']);
</script>

<template>
  <li>
    <h3 style="margin-block: 0">
      {{ education.name }}
    </h3>
    <small>{{ education.time }}</small>
    <p style="font-weight: 400;" v-html="education.description"></p>
  </li>
</template>
