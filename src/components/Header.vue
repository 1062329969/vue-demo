<template>
  <div id="header" class="header">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: 'header',
  props: ['va'],
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .header{
    width: 100%;
    height: 50px;
    border: 2px solid #69cc00;
    color: #0055cc;
    line-height: 50px
  }
</style>
