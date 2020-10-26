<template>
<div>
<h1>about Us</h1>
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur officia voluptatem mollitia deserunt dolores soluta nisi hic illo rerum, vitae sint nostrum labore. Modi ipsum perferendis fugit doloremque! Nesciunt, ratione!</p>
</div>

</template>
<script>
export default {
  head(){
    return{
      title : 'post | Aplication Nuxt ', 
      meta:[
        {
          hid: "description",
          name: "description", 
          content: "website about posts"
        }
      ],
      htmlAttrs:{
        lang: 'en'
      }
    }
  }
}
</script>