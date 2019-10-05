<template>
  <div class="hello">
    <h1>Home</h1>
    <router-link to="/discuss" tag="button">全部评价</router-link>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
  .hello
    width 100%
    height 100vh
    display flex
    flex-direction column
    justify-content space-around
    align-items center
</style>
