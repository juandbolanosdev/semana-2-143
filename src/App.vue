<template>
  <div id="app">

    <section-header></section-header>
    
    <main>
      <section-services></section-services>
      <div class="card border-light mb-3" style="max-width: 1200rem">
        <div class="card-header">
          <h3 class="section-text">Noticias</h3>
        </div>
        <div class="card-body">
          <section id="news">
            <div class="container-fluid">
              <section-api></section-api>
            </div>
          </section>
        </div>
      </div>

      <div class="card bg-light mb-3" style="max-width: 1200rem">
        <div class="card-header">
          <h3 class="section-text">Equipo</h3>
        </div>
        <div class="card-body">
          <section id="team">
            <div class="container-fluid">
              <div class="row justify-content-center mb-5">
                <div
                  class="col mt-5"
                  v-for="(item, index) of member"
                  :key="index"
                >
                  <team-card v-bind:member="item"></team-card>
                </div>
              </div>
            </div>
          </section>
        </div>
      </div>
    </main>
    <section-footer></section-footer>
  </div>
</template>

<script>
import TeamCard from "./components/TeamCard.vue";
import SectionApi from "./components/SectionApi.vue";
import SectionServices from "./components/SectionServices.vue";
import SectionHeader from "./components/SectionHeader.vue";
import SectionFooter from "./components/SectionFooter.vue";

export default {
  name: "App",
  components: {
    TeamCard,
    SectionApi,
    SectionServices,
    SectionHeader,
    SectionFooter
  },

  data() {
    return {
      member: [
        {
          "codigo": 1,
          "nombre": "Angela Amaya",
          "descripcion":
            "Ingeniera catastral y geodesta de la universidad Distrital de Bogotá, apasionada a la naturaleza.",
          "rol": "Tester",
          "image": "./imagenes/Angela.jpeg",
        },
        {
          "codigo": 2,
          "nombre": "David Lopez",
          "descripcion":
            "Ingeniero Electrónico de la Universidad Javeriana Cali, 35 años de edad, apasionado por los deportes especialmente el futbol.",
          "rol": "Desarrollador frontend",
          "image": "./imagenes/David.jpeg",
        },

        {
          "codigo": 3,
          "nombre": "Miguel Tarazona",
          "descripcion":
            "Estudiante de física en la Universidad de Santander, 22 años de edad, apasionado por el senderismo y la naturaleza.",
          "rol": "Desarrollador backend",
          "image": "./imagenes/Miguel.png",
        },

        {
          "codigo": 4,
          "nombre": "Juan D. Bolaños",
          "descripcion":
            "Ingeniero en electrónica y telecomunicaciones de la universidad del Cauca",
          "rol": "Desarrollador backend",
          "image": "./imagenes/Juan.jpg",
        },
      ],
    };
  },
};
</script>

