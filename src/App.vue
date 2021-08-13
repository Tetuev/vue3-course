<template xmlns="http://www.w3.org/1999/html">
   <div>
     <div>
       <button v-on:click="addLike">Like</button>
       <button v-on:click="addDislike">DisLike</button>
     </div>
     <div>Кол-во лайков: <strong>{{likes}}</strong></div>
     <div>Кол-во дизлайков: <strong>{{dislikes}}</strong></div>
   </div>

</template>

<script>
export default {
  data(){
    return{
      likes: 0,
      dislikes: 5,
    }
  },
  methods:{
    addLike(){
     this.likes += 1;
    },
    addDislike(){
      this.dislikes += 1;
    }
  }
}
</script>

<style>

</style>

// Single file component