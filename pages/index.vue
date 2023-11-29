<template>
  <div id="app">
      <Hero />
     <Profile />   
     <Gallery/>
        <Services />
     

    

  </div>
</template>
<script>
  import Hero from "~/components/Hero.vue" 
  import Profile from "~/components/Profile.vue" 
   import Gallery from "~/components/Gallery.vue"
import Services from "~/components/Services.vue"


 
  export default {
    components:{
      Hero,
    Profile, 
   Services,
   Gallery,

    }
  }
</script>