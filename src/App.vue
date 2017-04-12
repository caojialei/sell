<template>
  <div id="app">
    <v-header>
      i am header
    </v-header>
    <div class="tab">
      <!--<div class="tab-item"><a v-link="{path:'/goods">商品</a></div>-->
      <!--<div class="tab-item"><a v-link="{path:'/goods">评论</a></div>-->
      <!--<div class="tab-item"><a v-link="{path:'/goods">商家</a></div>-->
      <div class="tab-item"><router-link to='/goods'>商品3</router-link></div>
      <div class="tab-item"><router-link to='/ratings'>评论2</router-link></div>
      <div class="tab-item"><router-link to='/seller'>商家2</router-link></div>
      <div class="tab-item"><router-link to='/seller'>鹏鹏最傻气</router-link></div>
      <div class="tab-item"><router-link to='/seller'>鹏鹏最傻+1</router-link></div>
      <div class="tab-item"><router-link to='/seller'>鹏鹏最傻+2</router-link></div>
      <div class="tab-item"><router-link to='/seller'>鹏鹏最傻+3</router-link></div>
    </div>
    <router-view></router-view>
  </div>
</template>

<script type="text/ecmascript-6">
  import header from './components/header/header.vue';

  export default{
    components: {
      'v-header': header
    }
  };
</script>

<style lang="stylus" rel="stylesheet/stylus">

  #app
    .tab
      display :flex
      width : 100%
      height :40px
      line-height :40px
      // border-bottom :1px solid rgba(7,17,27,.1)
      border-1px(rgba(7,17,27,.1))
      .tab-item
        flex :1
        text-align :center
        & > a
          display : block
          font-size: 14px
          color :rgb(77,85,93)
          &.active
            color :rgb(240,20,20)


</style>
