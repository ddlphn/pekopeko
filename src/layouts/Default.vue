<template>
  <div class="layout">
    <header class="header">
      <strong>
        <h1 class="header-brand"><g-link to="/">ペコペコ</g-link></h1>
        <!-- {{ $static.metadata.siteName }} -->
      </strong>
      <!-- <nav class="nav">
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/about/">About</g-link>
      </nav> -->
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

<style>
body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.5;
  background: #0d2538;
  color: white;
}

.layout {
  max-width: 760px;
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
}

.header-brand {
  font-size: 42px;
  font-weight: 200;
}

.nav__link {
  margin-left: 20px;
}

a {
  text-decoration: none;
  color: white;
}
</style>
