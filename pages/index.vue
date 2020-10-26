<template>
  <h1>welcome to my frish app</h1>
</template>

<script>
export default {
  head(){
    return{
      title : 'Aplication Nuxt post | home', 
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