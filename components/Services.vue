<template>
  <div>
    <div class="card-container">
      <div class="flex-container">
        <img class="card-two" src="../static/services-images/web-development.jpg" />

        <div style="display: flex; flex-direction: column; height: 60vh">

          <p class="services-text">
            Unlock the full potential of the digital realm with our expert web
            development services. We specialize in crafting custom,
            user-friendly websites and web applications tailored to your unique
            needs.Our team of experienced developers utilizes the latest
            technologies and best practices to ensure your online presence is
            not just functional but exceptional. Whether you're looking to build
            a dynamic e-commerce platform or a cutting-edge web application,
            we've got you covered.
          </p>
        
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
img {
  width: 400px;
  height: 400px;
}
.services-header {
  font-size: 18px;
  color: #d73818;
  margin-left: 200px;
}
.services-about-header {
  width: 70%;
  font-size: 20px;
  color: #32110b;
  margin: 0 auto;
  font-family: Arial, Helvetica, sans-serif;
  margin-left: 50px;
}
.services-about-text {
  width: 90%;
  line-height: 1.5;
  font-size: 18px;
  margin-left: 300px;
  font-family: Arial, Helvetica, sans-serif;
}
.flex-container {
  display: flex;
  flex: wrap;
  margin-left: 200px;
}
.card-container {
  height: 50vh;
  margin-top: 100px;
}

.services-text {
  width: 65%;
  line-height: 1.5;
  font-size: 18px;
  margin-left: 50px;
  font-family: Arial, Helvetica, sans-serif;
}

.sub-services-text {
  width: 90%;
  line-height: 1.5;
  font-size: 20px;
  color: #d73818;
  margin-left: 50px;
  font-family: Arial, Helvetica, sans-serif;
}

/* Adjust the height and background properties */

.card-two {
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  max-width: 30%;
  height:300px;
}

@media (max-width: 1000px) {
  .services-about-header {
    width: 65%;
    font-size: 20px;
    color: #32110b;
    margin: 0 auto;
    font-family: Arial, Helvetica, sans-serif;
    margin-left: 0px;
  }
  .services-about-text {
    width: 90%;
    line-height: 1.5;
    font-size: 18px;
    margin-left: 300px;
    font-family: Arial, Helvetica, sans-serif;
  }
  .card-two {
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  max-width: 70%;
}
  .card-container {
    height: 40vh;
  }
  .services-text {
    width: 70%;
    text-align: left;
    font-size:18px;
    line-height: 2;
  }
  img {
    margin-left: 0px;
  }
  .flex-container {
    display: flex;
    flex-direction: column;
    margin-left: 100px;
  }



  .sub-services-text {
    width: 90%;
    line-height: 1.5;
    text-align: left;
    font-size: 20px;
    color: #d73818;
    margin-left: -50px;
    font-family: Arial, Helvetica, sans-serif;
  }
}

@media (max-width: 1000px) {
  img {
    display: none;
  }
  .card-container {
    height: 40vh;
  }

  .services-about-header {
    width: 70%;
    font-size: 18px;
      color: #32110b;

    font-family: Arial, Helvetica, sans-serif;
  }
  .services-text {
    width: 60%;
    text-align: left;
    margin-left:50px;
    line-height:1.5;
    font-size: 12px;
    font-family: Arial, Helvetica, sans-serif;
  }
}

/* Position the footer at the bottom of the viewport */
/* You may need to adjust the styling for your specific footer element */
footer {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  background-color: #f0f0f0; /* Set your footer background color */
  text-align: center; /* Center the content within the footer */
}
</style>