<template>
  <div id="app">
    <HeaderDc />
    <ContentDc />
    <FooterDc />
  </div>
</template>

<script>
import FooterDc from './components/FooterDc.vue'
import ContentDc from './components/ContentDc.vue'
import HeaderDc from './components/HeaderDc.vue'
import './assets/css/style.scss'

export default {
  name: 'App',
  components: {
    HeaderDc,
    ContentDc,
    FooterDc
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Roboto', sans-serif;
}
</style>
