<template>
  <div>
    <v-footer color="#2a3947" padless>
      <v-row justify="center" align="center" no-gutters>

        <v-btn class="mx-4 white--text" icon>
          <v-icon size="24px">
            mdi-github
          </v-icon>
        </v-btn>        
        <v-btn class="mx-4 white--text" icon>
          <v-icon size="24px">
            mdi-gitlab
          </v-icon>
        </v-btn>        
        <v-btn class="mx-4 white--text" icon>
          <v-icon size="24px">
            mdi-facebook
          </v-icon>
        </v-btn>        
        <v-btn class="mx-4 white--text" icon>
          <v-icon size="24px">
            mdi-twitter
          </v-icon>
        </v-btn>        
        <v-btn class="mx-4 white--text" icon>
          <v-icon size="24px">
            mdi-instagram
          </v-icon>
        </v-btn>
        <v-btn class="mx-4 white--text" icon>
          <v-icon size="24px">
            mdi-discord
          </v-icon>
        </v-btn>
        
        <v-col class="py-4 text-center white--text" color="#142635" cols="12">
          {{ new Date().getFullYear() }} — <strong>Jesus Rafael Nava Cruz.</strong> Todos los derechos reservados
        </v-col>
      </v-row>
    </v-footer>
  </div>
</template>
<script>
export default {};
</script>