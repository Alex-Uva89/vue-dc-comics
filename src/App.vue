<template>
  <div id="app">
    <img alt="Dc logo" src="./img/dc-logo.png">
    <HeaderDc />
    <ContentDc />
  </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue'

export default {
  name: 'App',
  components: {
    HeaderDc,
    ContentDc,
  }
}
</script>

<style lang="scss">
#app {
  display: flex;
  justify-content: space-around;
  align-items: center;
  font-family: 'Roboto', sans-serif;
}
</style>
