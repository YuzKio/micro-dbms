<template>
  <div class="header">
    <div class="header-left">
      <div class="logo-font">micro DBMS front</div>
    </div>
    <div class="header-right">
      <a class="header-link">登录</a>
      或
      <a class="header-link">注册</a>
    </div>
  </div>
</template>

<script>
export default {
name: "HomeHeader"
}
</script>

<style lang="stylus" scoped>
  //1 rem = html font-size = 50px  在reset.css中定义的
  .header
    display: flex
    line-height: 1.2rem
    background: #0a0a0a
    opacity: 0.8
    color: #fff
    .header-left
      float: left
      .logo-font
        text-align: center
        font-size: .34rem
        margin-left: .32rem
    .header-right
      margin-left: auto
      text-align: right
      margin-right: .64rem
      .header-link
        color: #95c7b8
        &:hover
          cursor: pointer
          color: #e3f6f1
</style>