<template>
  <div id="app">
    <CoinInfo/>
  </div>
</template>

<script>
import CoinInfo from './components/CoinInfo.vue'

export default {
  name: 'app',
  components: {
    CoinInfo
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
