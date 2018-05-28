<template>
  <div id="footer" class="footer">
    111111111111111111
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: 'footer',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .footer{
    width: 100%;
    height: 50px;
    border: 2px solid #69cc00;
    color: #0055cc;
    line-height: 50px
  }
</style>
