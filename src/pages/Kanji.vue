<template>
  <Layout>

  <h2 class="kanji-list__subtitle">1</h2>

  <ul class="kanji-list">
    <li>一</li>
    <li>九</li>
    <li>七</li>
    <li>二</li>
    <li>人</li>
    <li>入</li>

    <li>八</li>
    <li>力</li>
    <li>十</li>
    <li>下</li>
    <li>三</li>
    <li>千</li>

    <li>上 </li>
    <li>口</li>
    <li>土</li>
    <li>夕</li>
    <li>大</li>
    <li>女</li>

    <li>子 </li>
    <li>小</li>
    <li>山</li>
    <li>川</li>
    <li>五</li>
    <li>天</li>

    <li>中 </li>
    <li>六</li>
    <li>円</li>
    <li>手</li>
    <li>文</li>
    <li>日</li>

    <li>月 </li>
    <li>木</li>
    <li>水</li>
    <li>犬</li>
    <li>王</li>
    <li>正</li>

    <li>出 </li>
    <li>本</li>
    <li>右</li>
    <li>四</li>
    <li>左</li>
    <li>玉</li>

    <li>生 </li>
    <li>田</li>
    <li>白</li>
    <li>目</li>
    <li>石</li>
    <li>立</li>

    <li>百 </li>
    <li>年</li>
    <li>休</li>
    <li>先</li>
    <li>名</li>
    <li>字</li>

    <li>早 </li>
    <li>気</li>
    <li>竹</li>
    <li>糸</li>
    <li>耳</li>
    <li>虫</li>

    <li>村 </li>
    <li>男</li>
    <li>町</li>
    <li>花</li>
    <li>見</li>
    <li>貝</li>

    <li>赤 </li>
    <li>足</li>
    <li>車</li>
    <li>学</li>
    <li>林</li>
    <li>空</li>

    <li>金 </li>
    <li>雨</li>
    <li>青</li>
    <li>草</li>
    <li>音</li>
    <li>校</li>
    <li>森</li>


  </ul>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Kanji'
  }
}
</script>

<style lang="scss">
  .kanji-list {
    padding-left: 0;

    &__subtitle {
      background: black;
      color: white;
      display: inline-block;
      border-radius: 50%;
      width: 35px;
      height: 35px;
      line-height: 35px;
      text-align: center;
    }

    li {
      list-style-type: none;
      display: inline-block;
      padding: 1rem;
      font-size: 32px;
    }
  }
</style>
