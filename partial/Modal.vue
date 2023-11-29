<template>
    <div class="container mx-auto">
         <div class="modal-overlay">
             <div class="modal ">     
               
                         <h1 class="text-base modal-text ">Thank you for downloading my resume!</h1>
                         <a class="close-btn" href="/">x</a>
                
            </div>
        </div>
    </div>
</template> 
<script>
    export default{
        
    }
</script>
<style scoped>

.modal-overlay {
margin-bottom:25px;
  display: flex;
  justify-content: center;
  padding:10px;
  
}
.modal-overlay:target{
  visibility: hidden;
}

.modal {
  position: relative;
  text-align: center;
  height: 40px;
  width: 450px;
  border-radius: 10px;
  margin-top: 40px;
  padding: 1em;
  background-color: #ff5733; /* Add the desired background color here */
}
.close-btn{

  margin-top:2px;
}
.modal-text{
  font-family: Arial, Helvetica, sans-serif;
  word-spacing: 2px;
  color:white;
  font-weight:bold;
  font-size:19px;
}
a{ 
  text-decoration: none;
  font-size:25px;
  color:white;
  position:absolute;
font-weight: bold;
  top:20px;
  left:25px;
}

@media (max-width: 760px) {
  .modal-overlay {
margin-bottom:25px;
  display: flex;
  justify-content: center;
 
  
}
.modal-overlay:target{
  visibility: hidden;
}

.modal {
  position: relative;
  text-align: center;
  height: 40px;
  width: 300px;
  border-radius: 10px;
  margin-top: 40px;
  padding: 0.5em;
  background-color: #ff5733; /* Add the desired background color here */
}
.close-btn{
  margin-top:2px;
}
.modal-text{

  font-size:12px;
}
a{ 
  text-decoration: none;
  font-size:16px;
  color:white;
  position:absolute;
font-weight: bold;
  top:10px;
  left:25px;
}

}



</style>