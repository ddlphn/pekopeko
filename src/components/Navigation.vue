<template>
  <nav class="nav">
    <g-link class="nav__link" to="/hiragana/">HIRAGANA</g-link>
    <g-link class="nav__link" to="/katakana/">KATAKANA</g-link>
    <!-- <g-link class="nav__link" to="/kanji/">KANJI</g-link>
    <g-link class="nav__link nav__link-dico" to="https://jisho.org/">DICO</g-link> -->
  </nav>
</template>

<script>
export default {
  name: 'Navigation',
}
</script>

<style lang="scss">
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
  padding-top: 2rem;
  padding-bottom: 2rem;
  max-width: 1100px;
  margin: 0 auto;

  &-brand {
    font-size: 42px;
    font-weight: 600;
    text-transform: uppercase;

    sup {
      font-size: 14px;
      font-weight: 200;
      position: absolute;
      top: 2.5rem;
    }
  }
}

nav {
  a {
    transition: all 0.3s;
    margin-left: 20px;

    // &-dico {
    //   color: white;
    //   background: #191F2B;
    //   text-transform: uppercase;
    //   padding-top: 0.2rem;
    //   padding-bottom: 0.2rem;
    //   padding-left: 0.8rem;
    //   padding-right: 0.8rem;
    //   font-weight: 600;
    //   font-size: 14px;
    //   border-radius: 8px;
    //   margin-right: 1rem;
    //   font-style: initial;
    //   transition: all 0.3s;
    // }

    &.active {
      font-weight: 600;
    }
  }
}
</style>