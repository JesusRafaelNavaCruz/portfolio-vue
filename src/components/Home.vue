<template>
  <section id="home">
    <v-container class="py-10 my-10">
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row align="center" justify="center">
            <v-col md="4">
              <h1 class="font-weight-regular text-uppercase mb-3">Hola</h1>
              <h1 class="display-2 font-weight-bold mb-4">Soy Jesus Nava</h1>
              <h1 class="font-weight-light mb-4">Desarrollador Web Front-End</h1>
              <v-btn dark large @click="$vuetify.goTo('#contact')">Contactame</v-btn>
            </v-col>
            <v-col md="6">
              <v-img src="@/assets/fotoPrincipal.png"></v-img>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>
<script>
export default {};
</script>