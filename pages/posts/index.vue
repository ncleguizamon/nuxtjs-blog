<template>
    <div>
      <h1>Post</h1>
      <Post 
        v-for="post of posts"
        v-bind:key="post.id"
        :name="post.title" 
        :id="post.id" />
        
    </div>

</template>

<script>
import axios from 'axios';
import Post from '../../components/Post';

export default {
    components:{
       Post
    },
    data(){
        return{
            posts:[]
        }
    },
    async created() {
       try{
               const res = await  axios.get('https://jsonplaceholder.typicode.com/posts')
                console.log(res)
                this.posts = res.data

       }catch(error){
          console.log(error)
       }

    }
}
</script>