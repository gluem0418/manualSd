<script setup lang="ts">
import TitleFlame from '@/components/TitleFlame.vue'
// import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <!-- <header> -->
  <TitleFlame class="title" :inside="'Manual'" />
  <!-- </header> -->

  <main>
    <!-- <TheWelcome /> -->
  </main>
</template>

<style scoped>
header {
  margin: 20px auto;
  width: 100%;
}

.title {
  margin: auto;
  display: block;
  /* margin: 50px auto; */
  /* width: 30%; */
}
</style>
