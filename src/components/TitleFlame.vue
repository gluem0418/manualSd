<template>
  <div class="flame">{{ inside }}</div>
</template>

<script setup lang="ts">

const props = defineProps({
  inside: { type: String },
});

</script>
<style scoped>
.flame {
  width: 500px;
  background-image: url('@/assets/img/flame1.png');
  background-size: 100% 100%;
  text-align: center;
  padding: 3.8vh 2vw;
  font-family: 'Aboreto';
  color: #F5F5F5;
  font-size: 48px;
}
</style>