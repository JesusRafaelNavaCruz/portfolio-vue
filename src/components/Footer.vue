<template>
  <div>
    <v-footer color="black lighten-1" padless>
      <v-row justify="center" no-gutters>
        
      <v-btn text rounded class="my-2" color="white"> Inicio </v-btn>

      <v-btn text rounded class="my-2" color="white"> Sobre mi </v-btn>

      <v-btn text rounded class="my-2" color="white"> Habilidades </v-btn>

      <v-btn text rounded class="my-2" color="white"> Servicios </v-btn>

      <v-btn text rounded class="my-2" color="white"> Portafolio </v-btn>

      <v-btn text rounded class="my-2" color="white"> Testimonios </v-btn>

      <v-btn text rounded class="my-2" color="white"> Blog </v-btn>

      <v-btn text rounded class="my-2" color="white"> Contacto </v-btn>


        <v-col class="black lighten-2 py-4 text-center white--text" cols="12">
          {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
        </v-col>
      </v-row>
    </v-footer>
  </div>
</template>
<script>
export default {};
</script>