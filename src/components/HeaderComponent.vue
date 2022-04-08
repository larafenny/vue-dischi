<template>
  <header>
      <div class="logo">
          <img src="@/assets/img/spotify-logo.png" alt="logo">
      </div>
  </header>
</template>

<script>
export default {
    name: 'HeaderComponent',

}
</script>

<style lang="scss" scoped>
    header{
        background-color: #2e3a46;
        height: 60px;
        .logo{
            padding: 10px;
            height: 100%;
            img{
            max-height: 100%;
        }
        }
        
    }
</style>