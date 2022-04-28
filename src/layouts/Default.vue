<template>
  <div id="app">
    <header class="header">
      <HeaderBrand />
      <Navigation />
    </header>

    <main class="main">
      <slot/>
    </main>

    <footer class="footer">
      <Footer />
    </footer>
  </div>
</template>

<script>
import Footer from '~/components/Footer.vue'
import Navigation from '~/components/Navigation.vue'
import HeaderBrand from '~/components/HeaderBrand.vue'

export default {
  components: {
    Footer,
    Navigation,
    HeaderBrand,
  },
}
</script>

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

main {
  max-width: 1100px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}

a {
  text-decoration: none;
  color: black;
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
