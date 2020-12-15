<template>
  <div id="app">
    <imagen-banner> </imagen-banner>
    <services-sections> </services-sections>

    <!-- news -->
    <div class="container-fluid">
      <news-sections> </news-sections>
    </div>

    <!-- members -->
    <div class="container-fluid">
        <div class="row justify-content-center mb-5">
          <team-card> </team-card>
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
  }
};
</script>

