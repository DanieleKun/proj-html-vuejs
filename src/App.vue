<template>
  <div id="app">
    <EPHeader/>
    <EPMain/>
    <EPFooter/>npm run serve
    
  </div>
</template>

<script>
import EPHeader from './components/EPHeader.vue'
import EPMain from './components/EPMain.vue'
import EPFooter from './components/EPFooter.vue'

export default {
  name: 'App',
  components: {
    EPHeader,
    EPMain,
    EPFooter
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
