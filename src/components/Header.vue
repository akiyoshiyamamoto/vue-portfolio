<template>
  <v-container class="d-flex justify-start mb-6">
    <router-link to="/" class="mr-5 grey--text">Home</router-link>
    <router-link to="/about" class="mr-5 grey--text">About</router-link>
    <router-link to="/works" class="mr-5 grey--text">Works</router-link>
    <router-link to="/contact" class="mr-5 grey--text">Contact</router-link>
  </v-container>

</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>
a {
  text-decoration: none;
  font-size: large;
}
</style>
