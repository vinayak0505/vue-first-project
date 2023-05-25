<template>
<div>

  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <posts-list></posts-list>
</div>
</template>



<script>
import PostsList from './components/PostsList.vue';
import HelloWorld from './components/HelloWorld.vue'
export default {
  name: 'App',
  components:{
    PostsList,
  HelloWorld
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
