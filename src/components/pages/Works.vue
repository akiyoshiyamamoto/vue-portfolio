<template>
  <v-container>
    <p class="text-sm-h5">担当した業務</p>
    <works-card
        title="hoge hoge"
        date="fuga fugaa"
        content="fugo fugo"
        class="mb-10"
    ></works-card>
    <works-card
        title="hoge hoge"
        date="fuga fugaa"
        content="fugo fugo"
        class="mb-10"
    ></works-card>
    <works-card
        title="hoge hoge"
        date="fuga fugaa"
        content="fugo fugo"
        class="mb-10"
    ></works-card>
    <works-card-with-img
        title="this is title"
        imageSrc="dog.png"
        imageAlt="犬の画像"
        year="2021-02-02"
        comment="this is comment area this is comment area this is comment area this is comment area this is comment area this is comment area this is comment area"
        url="https://github.com/akiyoshiyamamoto">
    </works-card-with-img>
  </v-container>
</template>

<script>
import WorksCard from "@/components/WorksCard";
import WorksCardWithImg from "@/components/WorksCardWithImg";

export default {
  name: "Works",
  components: {WorksCardWithImg, WorksCard},
}
</script>

<style scoped>

</style>
