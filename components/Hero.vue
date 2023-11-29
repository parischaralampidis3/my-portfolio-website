<template>
  <div class="">
    <div class="modal">
      <Modal v-show="showModal" />
    </div>

    <div class="hero-image">
      <div class="hero-header">
        <h1>Paris Charalampidis</h1>
        <div class="hero-text">
          <p>parou.char@gmail.com</p>
          <p>(+30)6947491008</p>
        </div>
      </div>

      <div>
        <a id="hero-modal" href="resume.pdf" @click="setNotification" download
          ><p class="button">Download Resume</p></a
        >
      </div>
    </div>
  </div>
</template>
  <script>
import Modal from "~/partial/Modal.vue";
export default {
  name: "Hero",
  components: {
    Modal,
  },
  data() {
    return {
      showModal: false,
    };
  },
  methods: {
    setNotification() {
      setTimeout(() => {
        this.showModal = true;
      }, 5000);
    },
  },
};
</script>
  <style scoped>
#hero-modal {
  visibility: block;
}
.hero-header {
  font-size: 20px;
  text-align: center;
  padding-top: 10px;
  color: white;
  font-weight: bold;
  font-family: Arial, Helvetica, sans-serif;
  margin-top: 20px;
  line-height: 1.5;
}
.hero-text {
  font-size: 18px;
  color: #fff;
  font-family: Arial, Helvetica, sans-serif;
  line-height:1.5;
}
a {
  text-decoration: none;
}
.hero-image {
  background-image: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.2)),
    url("~/static/cover-photo.jpg");
  height: 300px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  max-width: 80%;
  margin: 0 auto;
}
.button {
  text-align: center;
  font-weight: bold;
  width: 200px;
  margin:0 auto;
  color: #fff;
  font-size: 18px;
  padding: 10px;
  border-radius: 20px;
  background-color: #308cd8;
  box-shadow: 2px 3px 4px 1px rgba(0, 0, 0, 0.34);
  -webkit-box-shadow: 2px 3px 4px 1px rgba(0, 0, 0, 0.34);
  -moz-box-shadow: 2px 3px 4px 1px rgba(0, 0, 0, 0.34);
}



@media (max-width: 1000px) {
    .hero-header {
    font-size: 12px;
  }
  .hero-text {
    font-size: 12px;
  }

.button {
  margin:0 auto;
  width: 200px;

  font-size: 14px;
}
  
}

</style>