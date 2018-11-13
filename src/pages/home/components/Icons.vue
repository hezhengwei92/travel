<template>
    <div class="icons">
      <div class="icon">
        <div class="icon-img">
          <img  class="icon-img-content" src="http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png"/>
        </div>
        <p>热门景点</p>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HomeIcons'
}
</script>
<!-- 设定固定宽高比 因为 padding-bottom 是根据with 来计算的 -->
<style lang="stylus" scoped>
  .icons
    overflow: hidden
    height: 0
    padding-bottom: 50%
    background: green
    .icon
      position: relative
      overflow: hidden
      float: left
      width: 25%
      padding-bottom: 25%
      background: red
      .icon-img
        position: absolute
        top: 0
        left: 0
        right: 0
        bottom: .44rem
        background:blue
        .icon-imgcontent
          height :100%
</style>
