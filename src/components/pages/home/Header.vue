<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">
        &#xe624;
      </div>
    </div>
    <div class="header-input">
      <span class="iconfont">
        &#xe632;
      </span>输入城市/景点/游玩主题
    </div>
    <div class="header-right">
      城市
      <span class="iconfont arrow-icon">
      &#xe64a;
    </span>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'HomeHeader'
  }
</script>

<style lang="stylus" scoped>
  @import "~@/assets/style/varibles.styl"
  .header
    display: flex
    background-color:$bgColor
    line-height:0.86rem
    color:#fff
    .header-left
      width: 0.64rem
      float: left
      .back-icon
        text-align:center
        font-size 0.4rem
    .header-input
      background-color #fff
      flex: 1
      height 0.64rem
      line-height 0.64rem
      border-radius 0.1rem
      margin-left: 0.2rem
      margin-top :0.12rem
      padding-left: 0.2rem
      color:#ccc
    .header-right
      width:1.24rem
      float :right
      text-align: center
      .arrow-icon
        font-size 0.24rem
        margin-left:-0.01rem

</style>
