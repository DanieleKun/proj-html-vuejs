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
@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@200;300;400;500;700;900&display=swap');

*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

/* Scrollbar */
*::-webkit-scrollbar {
    width: 10px;
  }
  
  *::-webkit-scrollbar-track {
    background:#F7F8FA;
  }
  
  *::-webkit-scrollbar-thumb {
    background-color: #E56768;
    border-radius: 20px;
    border: 2px solid #E56768;
  }

a {
  text-decoration: none;
}
#app {
  // font-family: Avenir, Helvetica, Arial, sans-serif;
  // -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  // color: #2c3e50;
  // margin-top: 60px;
  font-family: 'Nunito', sans-serif;
}
</style>
