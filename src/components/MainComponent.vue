<template>
  <main>
    <div class="songs-container">

    </div>
  </main>
</template>

<script>
export default {
    name: 'MainComponent',
}
</script>

<style lang="scss" scoped>
    main{
        background-color: #1e2d3b;
        height: calc(100vh - 60px);

        .songs-container{
                  margin: 0 20%;
                  height: 100px
        }
    }
</style>

