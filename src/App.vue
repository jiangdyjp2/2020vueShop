<template>
<div i="app">
  <router-view/>
  <!--".meta.showFooter" defined in [router/index.js]-->
  <!--"$route"代表当前路由-->
  <FooterGuide v-show="$route.meta.showFooter" />
</div>
</template>

<script>
import FooterGuide from './components/FooterGuide/FooterGuide.vue'
export default {
  components: {
    FooterGuide
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .app
    width 100%
    height 100%
    background #f5f5f5
</style>
