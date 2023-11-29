<template>
  <div class="container mx-auto">
    <div
    style="margin-top:50px;"
      class="profile-container flex flex-col justify-center items-center lg:flex-row mt-10"
    >
      <div class="profile-card-one">
        <img class="avatar-image" src="~/static/avatar.jpg" />
      </div>

      <div class="profile-card-two mt-5 flex flex-col justify-around md:w-2/3">
        <div class="text-center lg: mt-6">
          <div class="profile-heading">
            <h1>
              Welcome to my digital playground!! My name is Paris Charalampidis!
            </h1>
          </div>
          <div class="profile-subheading">
            <p>Full Stack Engineer</p>
          </div>
          <div
            class="profile-text mt-6 text-left text-sm leading-6 mx-auto md:mx-auto w-2/3"
          >
            <p class="leading-6">
              I'm Paris Charalampidis, a passionate web developer hailing from
              the vibrant city of Athens, Greece.
            </p>
            <p class="leading-6">
              I thrive on harnessing the power of technology to craft immersive
              web experiences and bring creative visions to life. My mission is
              simple: to transform ideas into captivating digital realities.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
  <style scoped>
.section {
  padding-left: 20px;
  padding-right: 20px;
}
.profile-container {
  display: flex;
  flex-direction: row;
  justify-content: center;


}
.profile-heading {
  letter-spacing: 1px;
  width: 400px;
  margin-left: 50px;
  color: #d73818;
  font-size: 16px;
  font-family: Arial, Helvetica, sans-serif;
}
.profile-card {
  margin-left: 100px;
}
.avatar-image {
  width: 150px;
  height: 150px;
  border-radius: 50%;
}
.profile-text {
  width: 500px;
  margin-left: 50px;
  font-size: 18px;
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.5;
}
.profile-button {
  box-shadow: 2px 3px 4px 1px rgba(0, 0, 0, 0.14);
  -webkit-box-shadow: 2px 3px 4px 1px rgba(0, 0, 0, 0.14);
  -moz-box-shadow: 2px 3px 4px 1px rgba(0, 0, 0, 0.14);
}
.profile-btn {
  width: 200px;
  padding: 10px;

  font-size: 14px;
  font-family: Arial, Helvetica, sans-serif;
  margin-left: 50px;
  background-color: #308cd8;

  border-radius: 10px;
}
a {
  text-decoration: none;
  color: white;
  font-weight: bold;
  font-size: 18px;
}
.profile-subheading {
  font-weight: bold;
  font-size: 22px;
  margin-left: 50px;
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
@media (max-width:1000px) {
  .avatar-image {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  margin-right:100px;
}
  .profile-container {
    height: 90vh;
      display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  }
  .avatar-image {
    width: 150px;
    height: 150px;
    margin-left: 100px;
  }
  .profile-text {
  padding:30px;
  width: 300px;
  margin-left: 10px;
  margin-top:20px;
  font-size: 12px;
}
  .profile-heading {
    max-width: 300px;
    text-align: left;
    letter-spacing: 1px;
    width: 350px;
    color: #d73818;
    font-size: 12px;

    font-family: Arial, Helvetica, sans-serif;
  }
  .profile-btn {
  width: 200px;
  padding: 10px;

  font-size: 14px;
  font-family: Arial, Helvetica, sans-serif;
  margin-left: 150px;
  background-color: #308cd8;

  border-radius: 10px;
}
  .profile-subheading {
    margin-left: 50px;
    font-size:14px;
  }
  .profile-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-top: 0px;
  }
}
</style>