<script setup lang="ts">

import imgBase from "@/assets/img/imgBase.png"

import iconParty from "@/assets/icon/party.png"
import iconGuild from "@/assets/icon/guild.png"
import iconDungeon1 from "@/assets/icon/forest.png"

import iconDungeon2 from "@/assets/icon/swamp.png"
import iconDungeon3 from "@/assets/icon/desert.png"
import iconDungeon4 from "@/assets/icon/cave.png"
import iconDungeon5 from "@/assets/icon/palace.png"
import iconDungeon6 from "@/assets/icon/volcano.png"
import iconDungeon7 from "@/assets/icon/tower.png"

const iconTable = [
  iconDungeon2,
  iconDungeon3,
  iconDungeon4,
  iconDungeon5,
  iconDungeon6,
  iconDungeon7,
]

</script>

<template>
  <div class="base">

    <div class="contents">

      <div class="title">拠点での機能</div>

      <img class="imgBase" :src="imgBase" alt="Base" />

      <div class="mainSec">

        <!-- パーティ -->
        <div class="flexItem1">
          <img class="imgIcon" :src="iconParty" alt="Party" />
          <div>
            <div class="flexItem2">
              <div class="midTitle1">パーティ</div>
              <div class="text">パーティメンバーの状態確認、装備の変更が可能です。</div>
            </div>
          </div>
        </div>

        <!-- ギルド -->
        <div class="flexItem1">
          <img class="imgIcon" :src="iconGuild" alt="Guild" />
          <div>

            <div class="flexItem2">
              <div class="midTitle1">ギルド</div>
              <div class="text">パーティメンバーの状態確認、装備の変更が可能です。</div>
            </div>

            <div class="flexItem2">
              <div class="midTitle2">Add a Member</div>
              <div class="text">指定したメンバーをパーティに参加させます。（メンバーが4人の場合は参加出来ません。）</div>
            </div>

            <div class="flexItem2">
              <div class="midTitle2">Remove Member</div>
              <div class="text">指定したメンバーをパーティから解除します。（リーダーは解除出来ません。）</div>
            </div>

          </div>
        </div>

        <!-- ダンジョン -->
        <div class="flexItem1">
          <img class="imgIcon" :src="iconDungeon1" alt="Forest" />
          <div>
            <div class="flexItem2">
              <div class="midTitle1">ダンジョン</div>
              <div class="text">入るたびに違った構造になるダンジョンです。</div>
            </div>
            <div class="iconList">
              <div v-for="(icon, index) in iconTable" :key="index">
                <img :src="icon" alt="Dungeon" class="iconMini" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.base {
  position: relative;
  margin: 0 auto;
  width: 90%;
  background: #40424C;
  border-radius: 30px;
  border: 4px ridge #F5F5F5;
  padding: 50px 0;

}


.contents {
  width: 90%;
  margin: 0 auto;
  text-align: center;
}


.title {
  margin-bottom: 50px;
  font-size: 36px;
}

.imgBase {
  margin: 0 auto 50px;
  width: 90%;
  border-radius: 20px;
}
.mainSec {
  margin: 0 auto;
  width: fit-content;
}

.flexItem1 {
  display: flex;
  align-items: center;
  margin-bottom: 50px;
  gap: 3%;
  text-align: left;
  /* border: 1px dotted #F5F5F5; */
}

.flexItem2 {
  display: flex;
}

@media screen and (max-width: 800px) {}


.midTitle1 {
  width: 170px;
  font-size: 20px;
  margin-bottom: 20px;
  white-space: nowrap;
}

.midTitle2 {
  width: 170px;
  font-size: 18px;
  white-space: nowrap;
  /* border: 1px dotted #cfc9d7; */
}

.text {
  /* border: 1px dotted #cfc9d7; */
}

.iconList {
  display: flex;
  gap: 3%;
}
</style>
