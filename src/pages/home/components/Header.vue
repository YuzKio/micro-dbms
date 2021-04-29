<template>
  <div class="header">
    <div class="header-left">
      <div class="logo-font">LOGO slot</div>
    </div>
    <div class="header-right">
      <div>登录</div>
      或
      <div>注册</div>
    </div>
  </div>
</template>

<script>
export default {
name: "Header"
}
</script>

<style lang="stylus" scoped>
  .header
    display: flex
    line-height: .86rem
    background: #00bcd4
    color: #fff
    .header-left
      width: .64rem
      float: left
      .logo-font
        text-align: center
        font-size: .4rem
    .header-right
      min-width: 1.04rem
      padding: 0 .1rem
      float: right
      text-align: center
      color: #fff
</style>