<template>
  <span class="footer__copyright">{{ new Date().getFullYear() }} </span>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<style lang="scss">
.footer {
  max-width: 1100px;
  margin: 0 auto;
  text-align: right;
  padding-top: 2rem;
}
</style>