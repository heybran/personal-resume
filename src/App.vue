<script setup>
// Components
import ResumeSection from "./components/ResumeSection.vue";
import Highlights from "./components/Highlights.vue";
import Experiences from "./components/Experiences.vue";
import Certificates from "./components/Certificates.vue";
import Projects from "./components/Projects.vue";
import Educations from "./components/Educations.vue";
import ResumeHeader from "./components/ResumeHeader.vue";

// Data
import projects from "./data/projects.json";
import educations from "./data/educations.json";
import highlights from "./data/highlights.json";
import experiences from "./data/experiences.json";
import certificates from "./data/certificates.json";
import authorImage from "./assets/author.jpg";
import introduction from "./data/introduction.json";
</script>

<template>
  <ResumeHeader :name="introduction.name" :authorImage="authorImage" :description="introduction.description" />

  <ResumeSection heading="Highlights">
    <Highlights :highlights="highlights" />
  </ResumeSection>

  <ResumeSection heading="Experiences">
    <Experiences :experiences="experiences" />
  </ResumeSection>

  <ResumeSection heading="Certificates">
    <Certificates :certificates="certificates" />
  </ResumeSection>

  <ResumeSection heading="Projects">
    <Projects :projects="projects" />
  </ResumeSection>

  <ResumeSection heading="Education">
    <Educations :educations="educations" />
  </ResumeSection>
</template>

<style scoped>
</style>
