<template>
  <div id="app">
    <Header/>
    <Main/>
    <DiskList/>
  </div>
</template>

<script>
import Header from './components/HeaderComponent.vue'
import Main from './components/MainComponent.vue'
import DiskList from './components/DiskList.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    DiskList
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
}
</style>
