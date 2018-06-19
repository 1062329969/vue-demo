<template>
  <div class="hello">
    <ul >
      <li v-for="vo in list">
        name:{{vo.name}}
        <br>
        <span>sex:{{vo.email}}</span>
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
    name: 'HelloWorld',
    data () {
      return {
        list: []
      }
    },
    created(){
      this.$http.get('http://jsonplaceholder.typicode.com/users').then((data)=>{
          this.list = data.body
        })
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
