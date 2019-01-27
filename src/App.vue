<template>
  <div id="app">
    <v-header></v-header>
    <div class="tab">
      <div class="tab-item">
        <router-link to="/goods">
          <a>商品</a>
        </router-link>
      </div>
      <div class="tab-item">
        <router-link to="/ratings">
          <a>评价</a>
        </router-link>
      </div>
      <div class="tab-item">
        <router-link to="/seller">
          <a>商家</a>
        </router-link>
      </div>
    </div>
    <router-view></router-view>
  </div>
</template>

<script type="text/ecmascript-6">
  import header from './components/header/header'

  export default {
    components: {
      'v-header': header
    }
  }
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .tab
    display: flex;
    width: 100%;
    height: 40px;
    line-height: 40px;

    .tab-item
      flex: 1;
      text-align: center;
</style>
