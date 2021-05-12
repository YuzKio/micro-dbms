<template>
  <div>
    <home-header></home-header>
    <home-body></home-body>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeHeader from "@/pages/home/components/Header";
import HomeBody from "@/pages/home/components/Body"
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeBody
  }
}
</script>

<style lang="stylus">
</style>