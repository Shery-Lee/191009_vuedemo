<template>
  <div id="app">
    <router-view></router-view>
    <FooterGuide v-show="$route.meta.showfooter"></FooterGuide>
  </div>
</template>

<script>
  import FooterGuide from './components/FooterGuide/Footerguide'
  // import {reqCategorys} from "./api";
  export default {
    components: { FooterGuide },
    // async mounted () {  // 例子
    //   const result = await reqCategorys()
    //   console.log(result) // 打印输出
    // }
  }
</script>

<style lang="stylus" rel="stylesheet/stylus">
  #app
    width 100%
    height 100%
    background #f5f5f5
</style>
