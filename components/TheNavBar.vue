<template>
      <v-container>
        <v-row>
          <v-col cols="12" xs="12" sm="6" md="4">
            <v-app-bar app>
              <v-tabs fixed-tabs background-color="grey darken-3" dark centered>
                <v-tab v-for="(link, index) in links" :key="index" @click="goTo(link.id)">
                  {{ link.title }}
                </v-tab>
              </v-tabs>
            </v-app-bar>
          </v-col>
        </v-row>
      </v-container>
</template>

<script>
export default {
  data () {
    return {
      links: [
      { id: "tecnologies", title: "Tecnologías" },
      { id: "projects", title: "Projectos" },
      { id: "contact", title: "Contacto" },
    ],
    }
  },
  methods: {
    goTo(id) {
      let element = document.getElementById(id);
      element.scrollIntoView({ behavior: "smooth", block: "start" });
    },
  },
};
</script>

<style scoped>
.bc-black {
  background-color: black;
}
</style>