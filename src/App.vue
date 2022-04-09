<template>
  <div id="app">
    <Header/>
    <Main/>
    <DiskList :url="apiUrl"/>
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
    },
    data(){
      return{
          apiUrl: 'https://flynn.boolean.careers/exercises/api/array/music'
      }
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
