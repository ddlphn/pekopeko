<template>
  <Layout>

  <div>
    <h1>KATAKANA</h1>
    <ul class="alphabet-list">
      <li>ア <sup>a</sup></li>
      <li>イ <sup>i</sup></li>
      <li>ウ <sup>u</sup></li>
      <li>エ <sup>e</sup></li>
      <li>オ <sup>o</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>カ <sup>ka</sup></li>
      <li>キ <sup>ki</sup></li>
      <li>ク <sup>ku</sup></li>
      <li>ケ <sup>ke</sup></li>
      <li>コ <sup>ko</sup></li>
      <li> | </li>
      <li>ガ <sup>ga</sup></li>
      <li>ギ <sup>gi</sup></li>
      <li>グ <sup>gu</sup></li>
      <li>ゲ <sup>ge</sup></li>
      <li>ゴ <sup>go</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>サ <sup>sa</sup></li>
      <li>シ <sup>shi</sup></li>
      <li>ス <sup>su</sup></li>
      <li>セ <sup>se</sup></li>
      <li>ソ <sup>so</sup></li>
      <li> | </li>
      <li>ザ <sup>za</sup></li>
      <li>ジ <sup>ji</sup></li>
      <li>ズ <sup>zu</sup></li>
      <li>ゼ <sup>ze</sup></li>
      <li>ゾ <sup>zo</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>タ <sup>ta</sup></li>
      <li>チ <sup>chi</sup></li>
      <li>ツ <sup>tsu</sup></li>
      <li>テ <sup>te</sup></li>
      <li>ト <sup>to</sup></li>
      <li> | </li>
      <li>ダ <sup>da</sup></li>
      <li>ヂ <sup>ji</sup></li>
      <li>ヅ <sup>zu</sup></li>
      <li>デ <sup>de</sup></li>
      <li>ド <sup>do</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>ナ <sup>na</sup></li>
      <li>ニ <sup>ni</sup></li>
      <li>ヌ <sup>nu</sup></li>
      <li>ネ <sup>ne</sup></li>
      <li>ノ <sup>no</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>ハ <sup>ha</sup></li>
      <li>ヒ <sup>hi</sup></li>
      <li>フ <sup>fu</sup></li>
      <li>へ <sup>he</sup></li>
      <li>ホ <sup>no</sup></li>
      <li> | </li>
      <li>バ <sup>ba</sup></li>
      <li>ビ <sup>bi</sup></li>
      <li>ブ <sup>bu</sup></li>
      <li>ベ <sup>be</sup></li>
      <li>ボ <sup>bo</sup></li>
      <li> | </li>
      <li>パ <sup>pa</sup></li>
      <li>ピ <sup>pi</sup></li>
      <li>プ <sup>pu</sup></li>
      <li>ぺ <sup>pe</sup></li>
      <li>ポ <sup>po</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>マ <sup>ma</sup></li>
      <li>ミ <sup>mi</sup></li>
      <li>ム <sup>mu</sup></li>
      <li>メ <sup>me</sup></li>
      <li>モ <sup>mo</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>ヤ <sup>ya</sup></li>
      <li>ユ <sup>yu</sup></li>
      <li>ヨ <sup>yo</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>ラ <sup>ra</sup></li>
      <li>リ <sup>ri</sup></li>
      <li>ル <sup>ru</sup></li>
      <li>レ <sup>re</sup></li>
      <li>ロ <sup>ro</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>ワ <sup>wa</sup></li>
      <li>ヲ <sup>o</sup></li>
    </ul>
    <ul class="alphabet-list">
      <li>ン <sup>n</sup></li>
    </ul>
  </div>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Katakana'
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
