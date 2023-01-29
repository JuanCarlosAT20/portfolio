<template>
  <v-container>
    <v-row>
      <v-col
        cols="12"
        xs="12"
        sm="6"
        md="4"
        lg="6"
        v-for="(project, i) in projects"
        :key="i"
      >
        <v-card class="mx-auto" max-width="500" outlined tile>
          <div align-center justify-center>
            <v-img
              max-height="500"
              max-width="500"
              contain
              :src="project.img"
            ></v-img>
          </div>
          <v-card-title>{{ project.name }}</v-card-title>
          <v-card-title class="black--text text-grey-darken-1 caption mt-n6">{{
            project.description
          }}</v-card-title>
          <div class="text-center black--text">
            <v-card-text class="text-h6">Tecnologías usadas</v-card-text>
          </div>
          <div class="d-flex justify-center">
                <v-icon x-large color="green">mdi-vuejs</v-icon>
                <v-icon x-large color="light-blue accent-1">mdi-vuetify</v-icon>
              </div>
          <v-card-actions class="d-flex justify-center">
            <a href="https://github.com/JuanCarlosAT20"
              ><v-icon color="white">mdi-github</v-icon></a
            >
            <a href="">DEMO</a>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          img: require("../assets/project1.jpg"),
          name: "Portafolio",
          description: "Portfolio personal para agregar projectos",
        },
      ],
    };
  },
};
</script>