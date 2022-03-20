<template>
  <Layout>

  <div>
    <h1>HIRAGANA</h1>
    <ul class="alphabet-list">
      <li>あ <sup>a</sup></li>
      <li>い <sup>i</sup></li>
      <li>う <sup>u</sup></li>
      <li>え <sup>e</sup></li>
      <li>お <sup>o</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>か <sup>ka</sup></li>
      <li>き <sup>ki</sup></li>
      <li>く <sup>ku</sup></li>
      <li>け <sup>ke</sup></li>
      <li>こ <sup>ko</sup></li>
      <li> | </li>
      <li>が <sup>ga</sup></li>
      <li>ぎ <sup>gi</sup></li>
      <li>ぐ <sup>gu</sup></li>
      <li>げ <sup>ge</sup></li>
      <li>ご <sup>go</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>さ <sup>sa</sup></li>
      <li>し <sup>shi</sup></li>
      <li>す <sup>su</sup></li>
      <li>せ <sup>se</sup></li>
      <li>そ <sup>so</sup></li>
      <li> | </li>
      <li>ざ <sup>za</sup></li>
      <li>じ <sup>ji</sup></li>
      <li>ず <sup>zu</sup></li>
      <li>ぜ <sup>ze</sup></li>
      <li>ぞ <sup>zo</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>た <sup>ta</sup></li>
      <li>ち <sup>chi</sup></li>
      <li>つ <sup>tsu</sup></li>
      <li>て <sup>te</sup></li>
      <li>と <sup>to</sup></li>
      <li> | </li>
      <li>だ <sup>da</sup></li>
      <li>ぢ <sup>dji</sup></li>
      <li>づ <sup>dzu</sup></li>
      <li>で <sup>de</sup></li>
      <li>ど <sup>do</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>な <sup>na</sup></li>
      <li>に <sup>ni</sup></li>
      <li>ぬ <sup>nu</sup></li>
      <li>ね <sup>ne</sup></li>
      <li>の <sup>no</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>は <sup>ha</sup></li>
      <li>ひ <sup>hi</sup></li>
      <li>ふ <sup>fu</sup></li>
      <li>へ <sup>he</sup></li>
      <li>ほ <sup>no</sup></li>
      <li> | </li>
      <li>ば <sup>ba</sup></li>
      <li>び <sup>bi</sup></li>
      <li>ぶ <sup>bu</sup></li>
      <li>べ <sup>be</sup></li>
      <li>ぼ <sup>bo</sup></li>
      <li> | </li>
      <li>ぱ <sup>pa</sup></li>
      <li>ぴ <sup>pi</sup></li>
      <li>ぷ <sup>pu</sup></li>
      <li>ぺ <sup>pe</sup></li>
      <li>ぽ <sup>po</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>ま <sup>ma</sup></li>
      <li>み <sup>mi</sup></li>
      <li>む <sup>mu</sup></li>
      <li>め <sup>me</sup></li>
      <li>も <sup>mo</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>や <sup>ya</sup></li>
      <li>ゆ <sup>yu</sup></li>
      <li>よ <sup>yo</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>ら <sup>ra</sup></li>
      <li>り <sup>ri</sup></li>
      <li>る <sup>ru</sup></li>
      <li>れ <sup>re</sup></li>
      <li>ろ <sup>ro</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>わ <sup>wa</sup></li>
      <li>を <sup>o</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>ん <sup>n</sup></li>
    </ul>
  </div>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Hiragana'
  }
}
</script>

<style lang="scss">
  .alphabet-list {
    padding-left: 0;

    li {
      list-style-type: none;
      display: inline;
      margin-right: 1rem;
      font-size: 28px;

      sup {
        font-size: 12px;
      }
    }
  }
</style>
