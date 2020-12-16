<template>
  <div>
    <!-- Image and text -->
    <nav class="navbar navbar-expand-lg sticky-top navbar-dark bg-info">
      <a class="navbar-brand" href="# ">
        <img
          src="https://www.lifeder.com/wp-content/uploads/2016/12/ramas-de-la-ciencia.png"
          width="30 "
          height="30
        "
          class="d-inline-block align-top"
          alt=" "
          loading="lazy "
        />
        Innovación y Ciencia
      </a>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav ">
        <ul class="navbar-nav">
          <li class="nav-item active">
            <a class="nav-link" href="# "
              >Inicio <span class="sr-only">(current)</span></a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#Servicios">Servicios</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#Noticias">Noticias</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#Miembros">Miembros</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#Contacto">Contacto</a>
          </li>
          
        </ul>
      </div>
    </nav>

    <!-- carousel -->
    <div
      id="carouselExampleCaptions"
      class="carousel slide"
      data-ride="carousel"
    >
      <ol class="carousel-indicators">
        <li
          data-target="#carouselExampleCaptions"
          data-slide-to="0"
          class="active"
        ></li>
        <li
          data-target="#carouselExampleCaptions"
          data-slide-to="1"
          class=""
        ></li>
        <li
          data-target="#carouselExampleCaptions"
          data-slide-to="2"
          class=""
        ></li>
      </ol>
      <div class="carousel-inner">
        <div class="carousel-item active">
         <img src="https://cdn.pixabay.com/photo/2018/07/15/10/44/dna-3539309_1280.jpg" alt="Foto" height="400" width="1600">
         
          <div class="carousel-caption d-none d-md-block">
            
            <p>Estudio de las técnicas modernas de obtención y procesamiento de datos.</p>
          </div>
        </div>
        <div class="carousel-item">
          <img src="https://cdn.pixabay.com/photo/2018/03/21/07/16/learning-3245793_1280.jpg" alt="Foto" height="400" width="1600">
          
          <div class="carousel-caption d-none d-md-block">
            <p>Proceso de enseñanza-aprendizaje basado en los principios de la neuropedagogía.</p>
          </div>
        </div>
        <div class="carousel-item">
          <img src="https://www.cs.duke.edu/sites/default/files/2019-06/datascience-banner1800x650.jpg" alt="Foto" height="400" width="1600">
          <div class="carousel-caption d-none d-md-block">
            
            <p>
              Bioestadística, análisis de datos y métodos estadísticos obtenidos en biología y medicina.
            </p>
          </div>
        </div>
      </div>
      <a
        class="carousel-control-prev"
        href="#carouselExampleCaptions"
        role="button"
        data-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
      </a>
      <a
        class="carousel-control-next"
        href="#carouselExampleCaptions"
        role="button"
        data-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
      </a>
    </div>
  </div>
</template>

<script>
export default {
    name:"ImagenBanner"

};
</script>

<style scoped>
</style>