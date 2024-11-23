<script setup lang="ts">

import imgDungeon from "@/assets/img/imgDungeon.png"

import iconBag from "@/assets/icon/bag.png"

</script>

<template>
  <div class="base">

    <!-- <div class="contents"> -->

    <div class="title">ダンジョン</div>

    <img class="imgMain" :src="imgDungeon" alt="Dungeon" />

    <!-- <div class="mainSec"> -->

    <div class="midTitle1">ダンジョン内での移動方法</div>

    <div class="flexItem1">
      <!-- キーボードでの操作 -->
      <div class="secItem1">
        <div class="midTitle2">キーボードでの操作</div>
        <table>
          <tbody>
            <tr>
              <td>↑</td>
              <td>前に進む</td>
            </tr>
            <tr>
              <td>D</td>
              <td>右を向く</td>
            </tr>
            <tr>
              <td>A</td>
              <td>左を向く</td>
            </tr>
            <tr>
              <td>↓</td>
              <td>後ろに下がる</td>
            </tr>
            <tr>
              <td>→</td>
              <td>右に水平移動</td>
            </tr>
            <tr>
              <td>←</td>
              <td>左に水平移動</td>
            </tr>
          </tbody>
        </table>
      </div>

      <div class="secItem1">
        <div class="midTitle2">クリック操作</div>
        <table>
          <tbody>
            <tr>
              <td>画面の中心</td>
              <td>前に進む</td>
            </tr>
            <tr>
              <td>画面の右側</td>
              <td>右を向く</td>
            </tr>
            <tr>
              <td>画面の左側</td>
              <td>左を向く</td>
            </tr>
            <tr>
              <td>扉・宝箱</td>
              <td>開ける</td>
            </tr>
            <tr>
              <td>石像</td>
              <td>調べる</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>

    <div class="flexItem2">

      <div>
        <img class="imgIcon" :src="iconBag" alt="Bag" />
      </div>

      <div>
        <div class="midTitle2">アイテムバッグ</div>
        <div class="text">「Magic Circle Of Return」を使用すると、拠点に戻ります。</div>
      </div>
    </div>

  </div>
</template>

<style scoped>
.base {
  position: relative;
  margin: 120px auto 0;
  width: 90%;
  text-align: center;
}

.title {
  font-size: 36px;
  display: flex;
  align-items: center;
  color: #EBA921;
}


.title:before,
.title:after {
  content: "";
  flex-grow: 1;
  height: 2px;
}

.title:before {
  margin-right: 30px;
  background: linear-gradient(to right, rgba(63, 66, 71, 0.3), #EBA921);
}

.title:after {
  margin-left: 30px;
  background: linear-gradient(to left, rgba(63, 66, 71, 0.3), #EBA921);
}

.imgMain {
  margin: 40px auto;
  width: 90%;
  border: ridge 3px #EBA921;
  border-radius: 20px;
}

/* .mainSec {
  margin: 0 auto;
  width: fit-content;
} */

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

table {
  margin: 14px 0;
  border-collapse: collapse;
}

table td {
  border: 1px solid #F5F5F5;
}

table tr td:nth-child(odd) {
  background: #3F4247;
  padding: 8px 50px
}

table tr td:nth-child(even) {
  padding: 8px 50px
}

.midTitle2 {
  font-size: 20px;
  text-align: left;
}

.flexItem2 {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 5%;
}
</style>
