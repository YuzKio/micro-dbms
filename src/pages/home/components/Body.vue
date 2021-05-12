<template>
 <div class="wrapper">
   <div class="bg-dynamic">
     <ul class="bg-bubbles">
<!--       <li v-for="(item, index) in bubbles" :key="index"></li>-->
       <li></li>
       <li></li>
       <li></li>
       <li></li>
       <li></li>
       <li></li>
       <li></li>
       <li></li>
       <li></li>
       <li></li>
     </ul>
   </div>
   <main class="main-content">
     <div class="title">
       <div style="font-size: 1.2rem;">micro DBMS front</div>
       <div style="font-size: 0.7rem;">高级数据库系统大作业</div>
     </div>
     <div class="button">
       <a class="btn-link">进入平台</a>
     </div>
   </main>
 </div>
</template>

<script>
export default {
  name: "HomeBody",
  props: {
    bubbles: Array
  },
  setup(props) {

  }
}
</script>

<style lang="stylus" scoped>
  .wrapper
    width: 100%
    position: absolute
    top: 1.2rem
    bottom: 0
    overflow: hidden;
    background: linear-gradient(to bottom right, #50A3A2, #53E3A6);
    .bg-dynamic
      .bg-bubbles
        li
          position: absolute
          bottom: 1.6rem
          width: 0.4rem
          height: 0.4rem
          background-color: rgba(255, 255, 255, 0.15)
          list-style: none
          animation: square 15s infinite
          transition-timing-function: linear
          &:nth-child(1)
            left: 10%
          &:nth-child(2)
            left: 20%
            width: 0.9rem
            height: 0.9rem
            animation-delay: 2s
            animation-duration: 7s
          &:nth-child(3)
            left: 25%
            animation-delay: 4s
          &:nth-child(4)
            left: 40%
            width: 0.4rem
            height: 0.6rem
            animation-duration: 8s
            background-color: rgba(255, 255, 255, 0.3)
          &:nth-child(5)
            left: 70%
          &:nth-child(6)
            left: 80%
            width: 1.2rem
            height: 1.2rem
            animation-delay: 3s
            background-color: rgba(255, 255, 255, 0.2)
          &:nth-child(7)
            left: 32%
            width: 1.6rem
            height: 1.6rem
            animation-delay: 2s
          &:nth-child(8)
            left: 55%
            width: 0.2rem
            height: 0.2rem
            animation-delay: 4s
            animation-duration: 15s
          &:nth-child(9)
            left: 25%
            width: 0.1rem
            height: 0.1rem
            animation-delay: 2s
            animation-duration: 12s
            background-color: rgba(255, 255, 255, 0.3)
          &:nth-child(10)
            left: 85%
            width: 1.6rem
            height: 1.6rem
            animation-delay: 5s
    .main-content
      //background: #fff
      .title
        text-align: center
        padding: 1.2rem 0
        line-height: 1.5rem
        color: rgba(255, 255, 255, 0.9)
      .button
        text-align: center
        margin: 0.5rem auto
        .btn-link
          font-size: 0.38rem
          padding: 0.4rem 0.5rem
          color: #fff
          border: solid 0.01rem rgba(255, 255, 255, 0.2)
          border-radius: 0.08rem
          &:hover
            cursor: pointer
            background-color: rgba(255, 255, 255, 0.2)

    @keyframes square
      0%
        opacity: 0.5
        transform: translateY(0) rotate(45deg)
      25%
        opacity: 0.75
        transform: translateY(-4rem) rotate(90deg)
      50%
        opacity: 1
        transform: translateY(-6rem) rotate(135deg)
      100%
        opacity: 0
        transform: translateY(-10rem) rotate(180deg)

</style>