<template>
   <div>
   <client-only>       
            <div class=" container mx-auto"> 
                <nav class="">
                    <ul class="navigation"> 
                        <nuxt-link class="nav-items contact-item" to="../navigation_pages/contact">Contact</nuxt-link>  
                    </ul>
                </nav>
                
            </div>
     </client-only>
    </div>
</template>
<style scoped>

ul li:hover{
    color:#bd1711;
}

a{
    color:black;
    text-decoration: none;
}
    .navigation{
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    a:hover{
    color:#5c5b5b
    }

    .nav-items {
      font-weight: bold;
      font-family: Arial, Helvetica, sans-serif;
      font-size: 24px;
    }
    .contact-item {
      margin-top: 20px;
    }
  



</style>