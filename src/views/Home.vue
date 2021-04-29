<template>
  <div class="home">
    <home-header></home-header>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeHeader from "@/pages/home/components/Header";

export default {
  name: 'Home',
  components: {
    HomeHeader
  }
}
</script>

<style lang="stylus">
.home
  margin: 0
  padding: 0
</style>