<script setup>
defineProps(['certificate']);
</script>

<template>
  <li>
    <h3 style="margin-block: 0">
      {{ certificate.name }}
    </h3>
    <small>{{ certificate.time }}</small>
    <p v-html="certificate.description"></p>
  </li>
</template>
