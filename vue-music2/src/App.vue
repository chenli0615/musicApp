<template>
  <div id="app">
    <m-header></m-header>
    <tab></tab>
    <keep-alive> <!-- keep-alive  将数据保存到缓存中 第二次再用的时候就不用再请求数据了 -->
      <router-view></router-view>
    </keep-alive>
    
  </div>
</template>

<script>
import MHeader from 'components/m-header/m-header'
import Tab from 'components/tab/tab'

export default{
  components:{
    MHeader,
    Tab
  }
}
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
  @import "~common/stylus/variable"

  #app
    color:$color-theme
</style>