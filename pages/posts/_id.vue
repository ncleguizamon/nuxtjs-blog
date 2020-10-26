<template>
    <div class="card">
    <h2>{{ post.title}}</h2>
    <p>Id : {{post.id}} </p>
    <p> Content :  {{ post.body}}</p>
    </div>
</template>


<script>
import axios from 'axios';
export default {
    data() {
        return {
           post: {}
        }
    },
    async created() {
       try{
               const res = await  axios.get('https://jsonplaceholder.typicode.com/posts/' + this.$route.params.id )
                console.log(res)
                this.post = res.data

       }catch(error){
          console.log(error)
       }

    }
}
</script>