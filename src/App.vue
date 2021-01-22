<template>
  <v-app>
    <Header/>
    <Menu/>
    <Content/>
    <Footer />
  </v-app>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Content from './components/Content.vue';
import Menu from './components/Menu.vue';

export default {
  components: { Header, Footer, Content, Menu },
  // components: { Header ,Footer},
  // components: { Header ,},
  name: "App",

  data: () => ({}),
};
</script>
