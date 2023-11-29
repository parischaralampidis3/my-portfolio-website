<template>
  <div>
    <div class="gallery-header">
      <h1>Gallery</h1>
    </div>

    <div class="card-container">
        <div>
          <h3 class="gallery-subtitle">Langshare</h3>
        </div>
        <div class="gallery-text">
          <p>
            Langshare is a full stack project. It consists an ERP project, that
            focuses to deliver efficient results, based on educative needs.This
            is a beta version that uses CRUD (Create,Read,Updae,Delete)
            methodology. So a user can create , update, and delete records that
            associated with personal information.
          </p>
          <p>
            Also a user can associate a student with a class, and he has the
            ability to search for students.
          </p>
          <p>
            Langsare uses vanilla PHP back-end technology and Javascript for
            delivering frontend functionality at the web app.Also I use Tailwind
            CSS as CSS library.In order the data to be saved and be fetched the
            proper way, i have intergrated the web app with MySQL Database.
          </p>
        </div>

        <div class="">
          <img
            class="gallery-image"
            src="../static/services-images/langshare_dashboard_screen.png"
            width="50%"
            alt="dashboard"
          />

          <br />
          <img
            class="gallery-image"
            style="margin-top: 50px"
            src="../static/services-images/langshare_form.png"
            width="50%"
            alt="dashboard"
          />
        </div>

        <div class="gallery-text">
          <h3 class="">Tags</h3>
          <div>
            <p>Vanilla PHP, Javascript, Tailwind CSS</p>
          </div>
        </div>

        <div class="gallery-text">
          <h3 class="">Repository</h3>
          <a href="https://bitbucket.org/curly-dev/langshare/src/master/"
            >https://bitbucket.org/curly-dev/langshare/src/master/</a
          >
        </div>




        <div class="">
          <h3 class="gallery-subtitle" style="margin-top:100px;">Product form</h3>
        </div>
        <div class="gallery-text" style="margin-top:50px;">
          <p>
            Product form is a backend project. It consists of a project that
            handles data inputs from a form. Those inputs are saved into a web
            service that uses xml technology. When the data are saved, then are
            being displayed at a table.
          </p>
          <p>
            The project makes CRUD (Create,Read,Updae,Delete) opeation. So a
            user can create , update, and delete records.
          </p>
        </div>

        <div>
          <img
            class="gallery-image"
            src="../static/services-images/create_product_form.png"
            width="50%"
            alt="dashboard"
          />

          <br />
          <img
            class="gallery-image" style="margin-top:50px;"
            src="../static/services-images/create_product_list.png"
            width="50%"
            alt="dashboard"
          />
        </div>

        <div class="gallery-text">
          <h3 class="">Tags</h3>
        
            <p>Vanilla PHP, Javascript, XML ,Tailwind CSS</p>
        

          <h3 class="">Repository</h3>
          <a href="https://bitbucket.org/curly-dev/create_product/src/master/"
            >https://bitbucket.org/curly-dev/create_product/src/master/</a
          >
        </div>

  
    </div>
  </div>
</template>
  <style scoped>


.gallery-header {
  font-size: 20px;
  color: #d73818;
  margin-left: 130px;
}
.gallery-image {
  padding:20px;
  margin: 0 auto;
margin-left: 300px;
}
.gallery-subtitle {
  margin-left: 140px;
  color: #000;
  font-size: 25px;
  font-family: Arial, Helvetica, sans-serif;
}
.gallery-text {
  line-height: 1.5em;
  width: 50%;
  font-size: 16px;
  margin-left:370px;
  font-family: Arial, Helvetica, sans-serif;
  line-height:1.5;
}



@media (max-width: 1000px) {

.gallery-header {
  font-size: 12px;
  color: #d73818;
   margin-left:50px;

}

.gallery-subtitle {
  margin-left:55px;
  font-size: 18px;
  font-family: Arial, Helvetica, sans-serif;
}
  .gallery-text {
  line-height: 2em;
  width: 40%;
  font-size: 12px;
  margin: 0 auto;
  font-family: Arial, Helvetica, sans-serif;
  line-height:1.5;
}

  .flex-items {
    height: 500px;
    margin: auto 0;
    width: 100%;
  }

  .gallery-image { 
    width: 65%;
    padding:10px;
margin-left:105px;
}
}
</style>