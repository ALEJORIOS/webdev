<script setup lang="ts">
import FirstSection from './components/First-section.vue';
import SecondSection from './components/Second-section.vue';
</script>

<template>
  <div class="app">
    <FirstSection/>
    <SecondSection/>
  </div>
</template>

<style scoped>
  .app {
    overflow: hidden;
    height: fit-content;
  }
</style>
