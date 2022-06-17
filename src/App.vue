<template>
  <div id="app">
    <EPHeader/>
    <EPMain/>
    <EPFooter/>

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
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
#app {
  // font-family: Avenir, Helvetica, Arial, sans-serif;
  // -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  // color: #2c3e50;
  // margin-top: 60px;
}
</style>
