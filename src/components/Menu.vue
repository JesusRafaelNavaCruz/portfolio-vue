<template>
  <div>
    <v-navigation-drawer v-model="drawer" app temporary>
      <v-list-item>
        <v-list-item-avatar>
          <v-img src="https://randomuser.me/api/portraits/men/78.jpg"></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title>Jesus Nava</v-list-item-title>
          <v-list-item-subtitle>Developer</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-home</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>Inicio</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-home</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>Sobre mì</v-list-item-title>
          </v-list-item-content>
        </v-list-item>        
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-home</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>Habilidades</v-list-item-title>
          </v-list-item-content>
        </v-list-item>        
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-home</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>Servicios</v-list-item-title>
          </v-list-item-content>
        </v-list-item>        
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-home</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>Portafolio</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar
      app
      color="#2a3947"
      :flat="flat"
      dark
      class="px-15"
      :class="{ expand: flat }"
    >
      <v-toolbar-title>
        <v-img src="" max-width="50px" />
      </v-toolbar-title>
      <v-spacer />
      <v-app-bar-nav-icon
        @click.stop="drawer = !drawer"
        class="mr-4"
        v-if="isXs"
      />
      <div v-else>
        <v-btn text @click="$vuetify.goTo('#home')">
          <span class="mr-2">Inicio</span>
        </v-btn>
        <v-btn text @click="$vuetify.goTo('#about')">
          <span class="mr-2">Sobre mi</span>
        </v-btn>
        <v-btn text @click="$vuetify.goTo('#skills')">
          <span class="mr-2">Habilidades</span>
        </v-btn>
        <v-btn text @click="$vuetify.goTo('#services')">
          <span class="mr-2">Servicios</span>
        </v-btn>        
        <v-btn text @click="$vuetify.goTo('#portfolio')">
          <span class="mr-2">Portafolio</span>
        </v-btn>
        <v-btn outlined text @click="$vuetify.goTo('#contact')">
          <span class="mr-2">Contactame</span>
        </v-btn>
      </div>
    </v-app-bar>
  </div>
</template>
<style scoped>
.v-toolbar {
  transition: 0.6s;
}
.expand {
  height: 80px !important;
  padding-top: 10px;
}
</style>

<script>
export default {
  data: () => ({
    drawer: null,
    isXs: false,
    items: [
      ["mdi-home-outline", "Home", "#hero"],
      ["mdi-information-outline", "Sobre", "#features"],
      ["mdi-download-box-outline", "Download", "#download"],
      ["mdi-currency-usd", "Preços", "#pricing"],
      ["mdi-email-outline", "Contatos", "#contact"],
    ],
  }),
  props: {
    color: String,
    flat: Boolean,
  },
  methods: {
    onResize() {
      this.isXs = window.innerWidth < 850;
    },
  },
  watch: {
    isXs(value) {
      if (!value) {
        if (this.drawer) {
          this.drawer = false;
        }
      }
    },
  },
  mounted() {
    this.onResize();
    window.addEventListener("resize", this.onResize, { passive: true });
  },
};
</script>