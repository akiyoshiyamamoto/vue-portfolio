<template>
  <v-card
      class="mx-auto"
  >
    <v-card-text>
      <p class="text-h4 text--primary">
        {{ title }}
      </p>
      <p>{{ date }}</p>
      <div class="text--primary">
        {{ content }}
      </div>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: "WorksCard",
  props: [
      'title',
      'date',
      'content',
  ],
}
</script>

<style scoped>

</style>
