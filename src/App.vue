<template>
  <div id="app">
    <img alt="Vue logo" src="https://vuejs.org/images/logo.png">
    <HelloWorld :msg="ttt"/>
    <div v-for="t in ttt">
      <Test :msg="t"/>
      </div>
      
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import Test from './components/test.vue';

export default {
  name: 'App',
  components: {
    HelloWorld, Test
  },
  data(){
    return {
      ttt:["Holger", "Vera", "Adrian", "JULIA"]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
