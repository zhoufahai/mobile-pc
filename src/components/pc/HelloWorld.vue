<template>
  <div class="pc">
    <h1>{{ msg }}</h1>
    <button @click="go">跳转到第二个页面</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'HelloWorld,I am PC'
    }
  },
  methods: {
    go () {
      this.$router.push({ path: '/secondPage' })
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
