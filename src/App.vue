<script setup lang="ts">

import TitleFlame from '@/components/TitleFlame.vue'
import InfoBase from '@/components/InfoBase.vue'
import InfoDungeon from '@/components/InfoDungeon.vue'
import InfoBattle from '@/components/InfoBattle.vue'

</script>

<template>

  <TitleFlame class="title" :inside="'Manual'" />

  <InfoBase />

  <InfoDungeon />

  <InfoBattle />

</template>

<style scoped>
.title {
  margin: 90px auto 60px;
}
</style>
