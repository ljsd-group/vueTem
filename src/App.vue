<script setup>
import { ref } from 'vue'

const stockList = ref('クリエイト・レストランツHD(3387)は配当+500円優待券で4%超、JR九州(9142)は1日乗り放題券+500円券5枚、ヤマダHD(9831)は1000円ごとに500円券が年3枚、リョーサン菱洋HD(167A)は配当+2000円カタログギフト、共英製鋼(5440)は長期保有で2000円QUOカード、ユニプレス(5949)は長期保有で優待ポイント増加、シード(7743)はコンタクトレンズ割引+3年保有で3000円ギフト、MUTOH HD(7999)は3000円の選べるギフト、サンワテクノス(8137)は2年保有で2000円QUOカード、アルファCo(3434)は300株で3000円カタログギフト。いずれも総合利回り4%以上の優良銘柄です。')

const trackEvent = (label) => {
  // Google Tag Manager 事件追踪
  if (window.dataLayer) {
    window.dataLayer.push({
      'event': 'conversion',
      'category': 'LINE',
      'action': 'click',
      'label': label
    })
  }
}
</script>

<template>
  <div class="container">
    <!-- 第一屏 -->
    <div class="screen">
      <!-- トップバナー画像 -->
      <img src="https://img.aimetaaid.com/jpas_03.png" alt="優待投資で勝つ！" class="header-image">
      
      <!-- プロフィール円形画像 -->
      <div class="profile-circle">
        <img src="https://img.aimetaaid.com/jpas_01.png" alt="桐谷さんのプロフィール画像">
      </div>
      
      <h2>桐谷さん厳選！2025年注目優待銘柄10選</h2>
      <p>優待生活のプロが選ぶ、2025年に買うべき高配当・優待銘柄をご紹介します。総合利回り4%以上の厳選銘柄で、あなたも株主優待生活を始めましょう！</p>
      
      <!-- LINEボタン -->
      <a href="https://link.ljsdstage.top/jpas" id="purchase" class="button line-button" @click="trackEvent('top_button')">
        <img src="https://img.aimetaaid.com/jpas_04.png" alt="桐谷さんのLINEを無料で追加して今週の優良株を受け取ろう">
      </a>
      
      <!-- 白いボックス内のコンテンツ -->
      <div class="white-box">
        <p>桐谷さん曰く「私が買うのは常に安い時に買うのを心がけています。特に年初来安値や上場来安値をチェックし、バーゲンセールの時に買うのがコツです。2024年は平均株価が市場最高値を更新し、8月に暴落があったことも良かった。暴落があるとバーゲンセールなので、いいものが安く買えるチャンスです！」</p>
      </div>
      
      <!-- LINEボタン（再掲） -->
      <a href="https://link.ljsdstage.top/jpas" class="button line-button" @click="trackEvent('mid_button')">
        <img src="https://img.aimetaaid.com/jpas_04.png" alt="桐谷さんのLINEを無料で追加して今週の優良株を受け取ろう">
      </a>
    </div>
    
    <!-- 第二屏 -->
    <div class="screen">
      <!-- 第2の大きな画像 -->
      <img src="https://img.aimetaaid.com/jpas_02.png" alt="桐谷さん厳選優待銘柄" class="main-image">
      
      <!-- 白いボックス（最後のコンテンツ） -->
      <div class="white-box">
        <p>2025年桐谷さん厳選の10銘柄：</p>
        <p>{{ stockList }}</p>
      </div>
      
      <!-- LINEボタン（最後） -->
      <a href="https://link.ljsdstage.top/jpas" class="button line-button" @click="trackEvent('bottom_button')">
        <img src="https://img.aimetaaid.com/jpas_04.png" alt="桐谷さんのLINEを無料で追加して今週の優良株を受け取ろう">
      </a>
      
      <!-- フッター -->
      <div class="footer">
        <p>免責事項: 当サイトで提供される情報は、一般的な投資情報であり、特定の個別投資のアドバイスや推奨を目的とするものではありません。投資はご自身の責任において行ってください。</p>
        <p>© 2025 株式優待生活情報 All Rights Reserved.</p>
      </div>
    </div>
  </div>
</template>

<style>
body {
  font-family: 'cwTeXMing', Arial, sans-serif;
  color: #ffffff;
  background-color: #2b608e;
  margin: 0;
  padding: 0;
  text-align: center;
}
.container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  padding-top: 100px;
}
.header-image {
  max-width: 100%;
  height: auto;
  border: 4px solid #ffd700;
  border-radius: 5px;
  margin-bottom: 10px;
}
.profile-circle {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  border: 3px solid #fff;
  margin: -60px auto 20px;
  overflow: hidden;
  position: relative;
  z-index: 2;
}
.profile-circle img {
  width: 100%;
  height: auto;
}
h2 {
  font-size: 28px;
  margin: 15px 0;
}
p {
  line-height: 1.6;
  margin: 15px 0;
}
.button {
  display: block;
  width: 100%;
  max-width: 600px;
  margin: 20px auto;
  padding: 0;
  background: none;
  border: none;
  cursor: pointer;
}
.button img {
  width: 100%;
  height: auto;
}
.white-box {
  background-color: #ffffff;
  color: #000000;
  padding: 20px;
  border-radius: 5px;
  margin: 20px 0;
  text-align: center;
}
.strategy-image {
  width: 100%;
  max-width: 750px;
  height: auto;
  margin: 20px 0;
  border-radius: 5px;
}
.main-image {
  width: 100%;
  max-width: 750px;
  height: auto;
  margin: 20px 0;
  border-radius: 5px;
}
.footer {
  font-size: 14px;
  color: #e5e6e4;
  margin-top: 30px;
  text-align: center;
}
.screen {
  margin-bottom: 30px;
  padding-bottom: 30px;
}
</style>
