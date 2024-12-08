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
  padding: 20px;
  font-family: 'Aboreto';
  color: #F5F5F5;
  font-size: 48px;
}

@media screen and (max-width: 600px) {
  .flame {
    width: 300px;
    font-size: 40px;
    padding: 16px;
  }
}


</style>
