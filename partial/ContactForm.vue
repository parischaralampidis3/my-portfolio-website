<template>
  <div class="contact-form">
    <form
      @submit.prevent="sendEmail"
      id="myForm"
      class=""
      action="#"
      method="POST"
    >
      <!-- Your form fields -->
      <div class="contact-items">
        <label class="contact-label" for="name">What's your name: </label>
        <input
          class="contact-input"
          type="text"
          id="name"
          name="name"
          v-model="formData.name"
          required
        />
      </div>

      <div class="contact-items">
        <label class="contact-label" for="reply_to">Your email:</label>
        <input
          class="contact-input"
          type="text"
          id="reply_to"
          name="reply_to"
          v-model="formData.reply_to"
          required
        />
      </div>

      <div class="contact-items ">
        <label class="contact-label" for="theme"
          >Tell us about your project:</label
        >

        <textarea
          class="contact-textarea"
          name="theme"
          id="theme"
          rows="4"
          cols="50"
          v-model="formData.theme"
          required
        ></textarea>
      </div>

      <button
        class="contact-button "
        type="submit"
      >
        Υποβολή
      </button>
    </form>
  </div>
</template>
<script>
import emailjs from "emailjs-com";

export default {
  data() {
    return {
      formData: {
        name: "",
        reply_to: "",
        theme: "",
      },
    };
  },
  methods: {
    sendEmail() {
      const form = document.getElementById("myForm"); // Get the form element by its ID
      const formData = new FormData(form); // Create a FormData object from the form

      const emailParams = {
        name: formData.get("name"),
        theme: formData.get("theme"),
        //reply_to: formData.get('reply_to') // Corrected field name
      };
      const emailjsAppIdKey = process.env.VUE_APP_EMAILJS_APP_ID_KEY;
      emailjs

        .sendForm(
          "service_j5cm49h", // Your Email.js service ID
          "template_dq0sgfc", // Your Email.js template ID
          form, // Pass the form element as the third parameter
          "qy8nZ-TUU3353t0af" // Use the variable directly
        )
        .then((response) => {
          alert("Email is sent successfully");
          console.log("Email sent successfully:", response);
          // Handle success, e.g., show a success message to the user
        })
        .catch((error) => {
          console.error("Email sending failed:", error);
          // Handle error, e.g., show an error message to the user
        });
    },
  },
};
</script>

<style scoped>

.contact-form {
  max-width: 100%;
  width: 50%;
  margin: 0 auto;
  height: 100%;
}
.contact-items {
  margin-top: 0px;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  font-family: Arial, Helvetica, sans-serif;
}
.contact-textarea {
  width: 70%;
  height:100px;
  margin-top:20px;
}
.contact-label {
  font-size: 21px;
  margin-top: 10px;
  padding: 10px;

}

.contact-input{
  max-width: 100%;
  width:50%;
  padding:10px;
  margin-bottom:30px;

}

.contact-button {
  max-width: 100%;
  margin-left: 250px;
margin-top:50px;
  width: 40%;
  padding: 10px;
  background-color: #308cd8;
  color: #fff;
  font-size: 16px;
  border-radius: 10px;
  font-family: Arial, Helvetica, sans-serif;
}
@media (max-width: 1000px) {
  form{
  margin-top:10vh;
  }
  .contact-label {
  font-size: 12px;
  margin-top: 1vh;
  padding: 0px;
}
.contact-input{
  max-width: 100%;
  width:50%;
  padding:10px;
}


.contact-button {
    max-width: 100%;
    margin-left: 180px;
    width:100px;
    background-color: #308cd8;
    color: #fff;
    font-size: 16px;
    border-radius: 10px;
    font-family: Arial, Helvetica, sans-serif;
  }

}
@media (max-width: 768px) {
  .contact-button {
    max-width: 100%;
    margin-left:100px;
    width:100px;
    background-color: #308cd8;
    color: #fff;
    font-size: 16px;
    border-radius: 10px;
    font-family: Arial, Helvetica, sans-serif;
  }

}

@media (max-width: 608px) {
  .contact-button {
    max-width: 100%;
    margin-left:80px;
    width:100px;
    background-color: #308cd8;
    color: #fff;
    font-size: 16px;
    border-radius: 10px;
    font-family: Arial, Helvetica, sans-serif;
  }

}
</style>




