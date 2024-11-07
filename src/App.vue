<script setup lang="ts">
import TitleFlame from '@/components/TitleFlame.vue'
import InfoBase from '@/components/InfoBase.vue'

</script>

<template>
  <TitleFlame class="title" :inside="'Manual'" />

  <InfoBase class="base" />


</template>

<style scoped>
.title {
  margin: 50px auto;
}

</style>
