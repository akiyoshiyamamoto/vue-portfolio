<template>
  <v-container class="pb-10">
    <v-row class="d-flex justify-end">
      <h1 class="font-italic font-weight-thin text-sm-h1">
        yaak
        <br>
        portfolio
        <br>
        site
      </h1>
    </v-row>
    <v-row class="d-flex justify-start">
      <v-img
          :src="require('../../assets/dog.png')"
      />
    </v-row>
  </v-container>
</template>

<script>
export default {
name: "Home"
}
</script>

<style scoped>

</style>
