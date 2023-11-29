<template>
    <div class="header-container">
        <h1 class="contact-header">Let's get in touch!</h1>
        <p class="contact-subheading">Have questions or interested in working together? Please feel free to reach out by filling out the contact form below.Please send a message and we will get back at you soon!</p>
    </div>

  </template>
  
  <script>
  export default {
  
  }
  </script>
  
  <style scoped>
  .header-container{
    margin-top:10vh;
  }
  .contact-header{
    text-align:center;
    font-size:22px;
    padding-top:40px;
    font-weight: bold;
    color:black;
    font-family:Arial, Helvetica, sans-serif;
  }
  .contact-subheading{
    line-height: 1.5;
    width:500px;
    font-size:18px;
    font-family:Arial, Helvetica, sans-serif;
    text-align: center;
    margin-top:50px;
    margin:0 auto;
    text-align:left;
  }

  @media (max-width:1000px) {

  .contact-header{
    text-align:center;
    font-size:12px;
  }
    .contact-subheading{
    line-height: 1.5;
    width:300px;
    font-size:12px;
    font-family:Arial, Helvetica, sans-serif;
    text-align: center;
    margin-top:50px;
    margin:0 auto;
    text-align:left;
  }
  }
  </style>
