<script setup>
defineProps(['project']);
</script>

<template>
  <li>
    <h3 style="margin-block: 0">
      {{ project.name }}
    </h3>
    <a :href="project.url">{{ project.url }}</a>
    <p v-html="project.description"></p>
  </li>
</template>
