<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入/城市/景点/游玩主题
    </div>
    <div class="header-right">
      {{this.city}}
      <span class="iconfont arrow-icon">&#xe64a;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    city: String
  }
}
</script>
<!-- 1rem = html font-size = 50px   2rem = html font-size = 100px   因为2倍图 86px 所以真实是43px = 43/50 = 0.86rem -->
<style lang="stylus" scoped>
  @import "~styles/varibles.styl"
  .header
    display flex
    line-height: .86rem
    background: $bgColor
    color: #fff
    .header-left
      width: .64rem
      float: left
      .back-icon
        text-align :center
        font-size :.4rem
    .header-input
      flex : 1
      height : .64rem
      line-height: .64rem
      margin-top : .12rem
      margin-left: .2rem
      padding-left : .2rem
      background:  #fff
      border-radius: .1rem
      color: black
    .header-right
      width: 1.24rem
      float:right
      text-align: center
      arrow-icon
        margin-left: -.04rem
        font-size:.24rem
</style>
