<template>
  <div id="app">
    hello vue stylus
    <img src="./assets/logo.png">
    <!-- <router-view></router-view> -->
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
  @import "~common/stylus/variable"
  #app
    color $color-theme
</style>
