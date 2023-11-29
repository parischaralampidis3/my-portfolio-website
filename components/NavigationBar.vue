<template>
  
        <div class="section">
        <div class="container mx-auto">
            <div class="py-12">
            <div class="navigation">
                    <div>
                        <nuxt-link to="/" class="home-link   hover:text-red-700  font-bold">Home</nuxt-link>
                    </div>
                    <nav id="nav" class="hidden lg:block font-semibold text-xl"> 
                       

                
                    <nuxt-link class="nav-items contact-item" to="../navigation_pages/contact">Contact</nuxt-link>  
            
                           
                    </nav> 
            </div>
        </div>
        </div>
    </div>


</template>
<script>

    export default{
        name:"NavigationBar",
        data(){
            return{
            isOpen: false
        }
        },
        methods: {
            handleClick(){
           this.isOpen = !this.isOpen
            }
        }
    }
</script>
<style scoped>
.home-link{
    font-size:2rem;
    font-weight: bold;
    font-family: Arial, Helvetica, sans-serif;
}
.nav-items{
      font-size:1.5rem;
    font-weight: bold;
    font-family: Arial, Helvetica, sans-serif;
}
.about-item{
    margin-right:10px;
}
.contact-item{
    margin-left:10px;
}
.navigation{
    padding:50px;
    display:block;
    display:flex;
    align-items:center;
    justify-content:space-between
  
}
.section{ 
    padding-left:50px;
    padding-right:50px;
}
nav > li a:hover{
    color: tomato;
}
a{
    text-decoration: none;
    color:black;
}

 @media (max-width:1000px) {
    .navigation{
        display:none;
    }


}


</style>