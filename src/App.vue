<template>
  <div id="app">
    <HeaderDc />
    <JumboDc />
    <ContentDc />
    <FooterDc />
  </div>
</template>

<script>
import JumboDc from './components/JumboDc.vue'
import FooterDc from './components/FooterDc.vue'
import ContentDc from './components/ContentDc.vue'
import HeaderDc from './components/HeaderDc.vue'
import './assets/css/style.scss'

export default {
  name: 'App',
  components: {
    HeaderDc,
    ContentDc,
    FooterDc,
    JumboDc
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Roboto', sans-serif;
}
</style>
