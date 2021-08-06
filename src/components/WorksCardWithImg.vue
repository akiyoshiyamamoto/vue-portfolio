<template>
  <v-card
      class="mx-auto"
  >
      <v-card-title>
        {{ title }}
      </v-card-title>
    <div>
      <v-container>
        <v-row>
          <v-col cols="auto"
                 class="d-flex">
            <v-avatar
                class="profile"
                color="grey"
                size="400"
                tile
            >
              <v-img
                  :src="src"
                  :alt="alt"
              ></v-img>
            </v-avatar>
            <div>
              <v-card-text>{{ year }}</v-card-text>
              <v-card-text>{{ comment }}</v-card-text>
              <v-btn icon :href="href">
                <v-icon>mdi-github</v-icon>
              </v-btn>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </v-card>
</template>

<script>
export default {
  name: "WorksCardWithImg",
  props: [
    'title',
    'imageSrc',
    'year',
    'comment',
    'url',
    'imageAlt',
  ],
  data() {
    return {
      src: require(`../assets/${this.imageSrc}`),
      alt: this.imageAlt,
      href: this.url
    }
  }
}
</script>

<style scoped>

</style>
