<script setup>
defineProps(['heading']);
</script>

<template>
  <section class="resume-section">
    <h2 class="resume-section__heading">{{ heading }}</h2>
    <slot></slot>
  </section>
</template>