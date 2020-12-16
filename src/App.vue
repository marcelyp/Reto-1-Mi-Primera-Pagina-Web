<template>
  <div id="app">
    <imagen-banner> </imagen-banner>
    <div id="Servicios" class="container-fluid">
    <h2>Servicios</h2>
    <services-sections> </services-sections>
    </div>

    <!-- news -->
    <div class="container-fluid" id="Noticias">
      <h2>Noticias</h2>
      <news-sections> </news-sections>
    </div>

    <!-- members -->
    <div class="container-fluid" id="Miembros">
      <h2>Miembros</h2>
      <div class="row justify-content-center mb-5">

        <div class="col mt-5" v-for="(miembro,index ) of Team" :key="index" >
            <team-card :member="miembro"> </team-card>
        </div>
      </div>   
    </div>

    <footer-sections> </footer-sections>
  </div>
</template>

<script>
import ImagenBanner from "./components/ImagenBanner.vue";
import ServicesSections from "./components/ServicesSections.vue";
import NewsSections from "./components/NewsSections.vue";
import TeamCard from "./components/TeamCard.vue";
import FooterSections from "./components/FooterSections.vue";

export default {
  name: "App",
  components: {
    ImagenBanner,
    ServicesSections,
    NewsSections,
    TeamCard,
    FooterSections,
  },
  data(){
    return{
    Team:
        [
        {
        codigo : 1,
        nombre : "Alejandro Zapata Alzate",
        descripcion: "Ingeniero de petróleos, aficionado de los videojuegos, amante de la comida y futuro programador",
        rol : "Desarrollador Backend",
        image: "https://i.imgur.com/6j8nrjq.png"
        },
        {
        codigo : 2,
        nombre : "Eduardo Malagón Puentes",
        descripcion: "Biólogo, Magíster en pedagogía. Docente, editor de textos de Ciencias Naturales. Hobbies: practicar ciclismo y atletismo, viajar, leer.",
        rol : "Desarrollador Backend",
        image: "https://i.imgur.com/piXalN2.png"  
        },
        {
        codigo : 4,
        nombre : "Marcela Cely Prieto ",
        descripcion: "Matemática de la Universidad Distrital Francisco Jose de Caldas, Analista de audiencias en Canal Trece. Pasatiempos favoritos, nadar y viajar. En la actualidad reside en Bogotá.",
        rol : "Scrum Master",
        image: "https://i.imgur.com/B7b7X8R.png"
        },
        {
        codigo : 5,
        nombre : "Andrés Zuluaga Estrada",
        descripcion: "Ingeniero mecánico. Comerciante, docente y freelancer. Apasionado por viajar, aprender y la tecnología.",
        rol : "Desarrollador Frontend",
        image: "https://i.imgur.com/kQQ3Pev.png"
        }
    ]

}
  }
};
</script>

<style>
.card{
  height: 100%;
}
h2{
  text-align: center;
  
  margin-top: 50px;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  background: #17a2b8;
  color: white;
}
</style>
