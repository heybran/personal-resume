<script setup>
import CertificateCard from "./CertificateCard.vue";
defineProps(['certificates']);
</script>

<template>
  <ul>
    <CertificateCard v-for="(item, index) in certificates" :key="index" :certificate="item" />
  </ul>
</template>