<template>
  <v-app>
    <Menu/>
    <v-main>
      <Home/>
      <About/>
      <Skills/>
      <Services/>
    </v-main>
    <v-scale-transition>
      <v-btn
        fab
        dark
        fixed
        bottom
        right
        color="secondary"
        @click="$vuetify.goTo('#home')"
      >
        <v-icon>mdi-arrow-up</v-icon>
      </v-btn>
    </v-scale-transition>
    <Footer/>    
  </v-app>
</template>

<script>
import Menu from '../src/components/Menu.vue'
import Footer from './components/Footer.vue';
import Home from './components/Home.vue';
import About from './components/About.vue';
import Skills from './components/Skills.vue';
import Services from './components/Services.vue';

export default {
  name: 'App',
  components: {
    Menu,
    Footer,
    Home,
    About,
    Skills,
    Services
  },

  data: () => ({
    //
  }),
};
</script>
