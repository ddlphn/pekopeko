<template>
  <div class="layout">
    <header class="header">
      <strong>
        <h1 class="header-brand"><g-link to="/">pekopeko <sup>ペコペコ</sup></g-link></h1>
        <!-- {{ $static.metadata.siteName }} -->
        <!-- <h2>日本語を習う</h2> -->
      </strong>
      <nav class="nav">
        <g-link class="nav__link" to="/hiragana/">HIRAGANA</g-link>
        <g-link class="nav__link" to="/katakana/">KATAKANA</g-link>
        <!-- <g-link class="nav__link" to="/kanji/">KANJI</g-link>
        <g-link class="nav__link nav__link-dico" to="https://jisho.org/">DICO</g-link> -->
      </nav>
    </header>
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style lang="scss">
body {
  margin: 0;
  padding: 0;
  line-height: 1.5;
  background: white;
  color: #333;
  font-family: 'Source Sans Pro', sans-serif;
}

.layout {
  max-width: 1100px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
  padding-top: 2rem;
  padding-bottom: 2rem;

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

a {
  text-decoration: none;
  color: black;
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

td {
  padding-right: 2rem;
}

th {
  text-align: left;
  font-size: 20px;
}

ul {
  padding-left: 1rem;
}
</style>
