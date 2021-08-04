<template>
  <v-app>
    <v-main>
      <Header></Header>
      <router-view></router-view>
      <Footer></Footer>
    </v-main>
  </v-app>
</template>

<script>

import Header from "@/components/Header";
import Footer from "@/components/Footer";
export default {
  name: 'App',

  components: {
    Footer,
    Header
  },

  data: () => ({
    //
  }),
};
</script>
