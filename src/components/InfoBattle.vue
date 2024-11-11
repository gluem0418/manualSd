<script setup lang="ts">

import imgBattle from "@/assets/img/imgBattle.png"

import iconOrb1 from "@/assets/icon/AttackOrb.png"
import iconOrb2 from "@/assets/icon/SkillOrb.png"

</script>

<template>
  <div class="base">

    <div class="title">バトル</div>

    <img class="imgMain" :src="imgBattle" alt="Battle" />

    <div class="flexItem1">
      <div class="secItem1">
        <img class="imgIcon" :src="iconOrb1" alt="AttackOrb" />
        <div class="text">通常攻撃</div>
      </div>
      <div class="secItem1">
        <img class="imgIcon" :src="iconOrb2" alt="SkillOrb" />
        <div class="text">スキルを使用します。（スキルには味方対象のスキルと敵対象のスキルがあります。）</div>
      </div>
    </div>

  </div>
</template>

<style scoped>
.base {
  position: relative;
  margin: 120px auto;
  width: 90%;
  text-align: center;
}

.title {
  font-size: 36px;
  display: flex;
  align-items: center;
  color: #DD5949;
}


.title:before,
.title:after {
  content: "";
  flex-grow: 1;
  height: 2px;
}

.title:before {
  margin-right: 30px;
  background: linear-gradient(to right, rgba(63, 66, 71, 0.3), #DD5949);
}

.title:after {
  margin-left: 30px;
  background: linear-gradient(to left, rgba(63, 66, 71, 0.3), #DD5949);
}

.imgMain {
  margin: 40px auto;
  width: 90%;
  border: ridge 3px #DD5949;
  border-radius: 20px;
}

.midTitle1 {
  font-size: 24px;
  margin-bottom: 24px;
}

.flexItem1 {
  margin-bottom: 30px;
  display: flex;
  justify-content: center;
  gap: 5%;
}

.secItem1 {
  display: flex;
  align-items:center;
  gap: 20px;
}

.text {
  text-align:left;
  min-width:100px;
  /* max-width:500px; */
}
</style>
