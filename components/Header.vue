<template>
   
    
    <div class="container mx-auto">
        <div class=" icons-container flex justify-between inset-x-0 fixed   z-10  mt-4 ml-0 mr-0 py-4 px-24 bg-white " >
                <div class="home"> 
               <a href="/">  <img  src="../static/home.svg" class="cursor-pointer" width="30"/> </a>
                </div>
                <div class="burger-menu">             
                    <img src="../static/burger-menu.svg" class="cursor-pointer" @click='handleClick' width="40">
                  
                </div>
            </div>
            <div class="  ">            
                <NavigationBar/> 
           </div>
            <div v-show="isOpen">
                <MobileMenu />
            </div>
        </div>
  
</template>
<script>
import NavigationBar from "~/components/NavigationBar.vue"
import MobileMenu from "~/partial/MobileMenu.vue"

export default{
    name:"Header",
    components:{
        NavigationBar,
        MobileMenu
    },
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
.home{
    display:none;
}
.burger-menu{
    display: none;
}

 @media (max-width:1000px) {

.home{
    display:block;
    margin-left:50px;
    margin-top:0px;
}
.icons-container{
    display:flex;
    justify-content: space-around;
    margin-top:20px;
}
.burger-menu{
   display:block
}


}
</style>