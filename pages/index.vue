<template>
  <v-app>
    <div>
<the-nav-bar />
    </div>
    <v-main  class="grey darken-3" app>
      <v-container fluid class="pa-0">
        <v-row no-gutters>
          <the-aside-information />
          <v-col cols="12" md="9">
            <v-card class="pa-2 grey darken-3" flat>
              <div class="text-center white--text">
                <h2>Hola, bienvenid@ a mi portfolio</h2>
              </div>
              <div class="white--text">
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Dolores quas ut rerum saepe, omnis voluptas impedit velit
                  ducimus, ipsum ad quo! Esse adipisci velit maiores molestias!
                  Expedita consequuntur accusantium eligendi. Lorem ipsum dolor
                  sit amet consectetur adipisicing elit. Voluptates sit
                  laudantium quidem ratione dignissimos, tempore hic
                  perspiciatis ea provident? Nisi provident molestias id sequi
                  dolore facere quas hic sint non! Lorem ipsum dolor sit amet
                  consectetur adipisicing elit. Dolores quas ut rerum saepe,
                  omnis voluptas impedit velit ducimus, ipsum ad quo! Esse
                  adipisci velit maiores molestias! Expedita consequuntur
                  accusantium eligendi. Lorem ipsum dolor sit amet consectetur
                  adipisicing elit. Voluptates sit laudantium quidem ratione
                  dignissimos, tempore hic perspiciatis ea provident? Nisi
                  provident molestias id sequi dolore facere quas hic sint non!
                </p>
              </div>
              <div id="tecnologies" class="mb-7 mt-7 text-center white--text">
                <h2>Tecnologías</h2>
              </div>
              <div class="d-flex justify-space-around">
                <v-icon x-large color="red">mdi-language-html5</v-icon>
                <v-icon x-large color="blue">mdi-language-css3</v-icon>
                <v-icon x-large color="yellow">mdi-language-javascript</v-icon>
                <v-icon x-large color="green">mdi-vuejs</v-icon>
                <v-icon x-large color="light-blue accent-1">mdi-vuetify</v-icon>
              </div>

              <div id="projects">
                <div class="mt-7 mb-7 text-center white--text">
                  <h2>Proyectos</h2>
                </div>
                <the-project-card />
              </div>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-main>

    <v-footer id="contact" color="grey darken-3" class="white--text">
      <v-row>
        <v-col cols="12">
          <div>
            <the-footer id="contacto"></the-footer>
          </div>
        </v-col>
      </v-row>
    </v-footer>
  </v-app>
</template>

<script>
import TheNavBar from "../components/TheNavBar.vue";
import TheProjectCard from "../components/TheProjectCard.vue";
import TheFooter from "../components/TheFooter.vue";
import TheAsideInformation from "../components/TheAsideInformation.vue";

export default {
  components: {
    TheNavBar,
    TheProjectCard,
    TheFooter,
    TheAsideInformation,
  },
};
</script>
