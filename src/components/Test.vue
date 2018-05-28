<template>
  <div class="test">
    <ul >
      <li v-for="vo in list" v-on:click="vo.show=!vo.show">
        name:{{vo.name}}
        <br>
        <span v-show="vo.show">sex:{{vo.sex}}</span>
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
    name: 'Test',
    data () {
      return {
        list: [
          {'name':111,'sex':222,'show':false},
          {'name':111,'sex':222,'show':false},
          {'name':111,'sex':222,'show':false},
          {'name':111,'sex':222,'show':false},
          {'name':111,'sex':222,'show':false},
          {'name':111,'sex':222,'show':false},
          {'name':111,'sex':222,'show':false},
          {'name':111,'sex':222,'show':false},
          {'name':111,'sex':222,'show':false},
          {'name':111,'sex':222,'show':false}
        ]
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .hello{
    margin: 20px;
  }
  ul{
    clear: both;
    overflow: hidden;
  }
  li{
    display: block;
    list-style: none;
    width: 15%;
    margin: auto 40px;
    float: left;
    border: 1px solid #000;
    min-height: 100px;
    line-height: 100px;
    margin-top: 50px;
  }
</style>
