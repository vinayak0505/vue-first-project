<template>
  <div class="list">
    postList
    <ul>
        <li v-for="post in posts" :key="post.id" class="">
            {{post.title}}
        </li>
    </ul>
  </div>
</template>

<script>

import axios from 'axios';
export default {
  name: 'PostsList',
  props: {
    msg: String
  },

  data(){
    return {
        posts:[]
    }
  },
  mounted(){
    axios.get('https://jsonplaceholder.typicode.com/todos').then((data) => {
        console.log(data);
        this.posts = data.data;
    })
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
