<script setup lang="ts">
import FirstSection from './components/First-section.vue';
import FourthSection from './components/Fourth-section.vue';
import SecondSection from './components/Second-section.vue';
import ThirdSection from './components/Third-section.vue';
</script>

<template>
  <div class="app">
    <FirstSection/>
    <SecondSection/>
    <ThirdSection/>
    <FourthSection/>
  </div>
</template>

<style scoped>
  .app {
    /* overflow: hidden; */
    height: fit-content;
    scroll-timeline-name: --colorTimeline;
  }
</style>