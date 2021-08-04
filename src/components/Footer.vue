<template>
  <v-container>
    <v-row class="d-flex justify-center">
      <router-link to="/" class="mr-5 grey--text text-decoration-none text-sm-caption">Home</router-link>
      <router-link to="/about" class="mr-5 grey--text text-decoration-none text-sm-caption">About</router-link>
      <router-link to="/works" class="mr-5 grey--text text-decoration-none text-sm-caption">Works</router-link>
      <router-link to="/contact" class="mr-5 grey--text text-decoration-none text-sm-caption">Contact</router-link>
    </v-row>
    <v-row>
      <v-col class="d-flex justify-center">
        <v-btn icon href="https://github.com/akiyoshiyamamoto">
          <v-icon>mdi-github</v-icon>
        </v-btn>
        <v-btn icon href="https://twitter.com/">
          <v-icon>mdi-twitter</v-icon>
        </v-btn>
      </v-col>
    </v-row>
    <v-col class="text-center grey--text text-sm-caption">
      {{ new Date().getFullYear() }} - <strong>yaak</strong>
    </v-col>
  </v-container>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style scoped>
</style>
