<template>
  <div id="app">
    <img src="./assets/logo.png">
    <!--<app-header></app-header>-->
    <!--<app-helloworld></app-helloworld>-->
    <!--<app-footer></app-footer>-->
    <ul>
      <li><router-link to="/">首页</router-link> </li>
      <li><router-link to="/demo">Demo</router-link> </li>
      <li><a href="/">首页</a> </li>
      <li><a href="/demo">Demo</a> </li>
    </ul>
    <router-view></router-view>
  </div>
</template>

<script>
import Footer from './components/Footer'
import Header from './components/Header'
import HelloWorld from './components/HelloWorld'

export default {
  name: 'app',
  components: {
    // "app-header":Header,
    // "app-helloworld":HelloWorld,
    // "app-footer":Footer,
  },
  methods:{

  }
}
</script>

<style>
  *{
    margin: 0;padding: 0;
  }
#app {
  text-align: center;
}
</style>
