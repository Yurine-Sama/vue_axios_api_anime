<template>
  <b-container fluid>
    <b-row>
      <b-col cols="3" v-for="anime in animelist.top" :key="anime">
        <Card :title="anime.title" :image="anime.image_url" />
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import Card from "@/components/Card.vue";
import axios from "axios";
export default {
  name: "Home",
  components: {
    Card
  },
  data() {
    return {
      animelist: {}
    };
  },
  mounted() {
    axios({
      method: "GET",
      url: "https://jikan1.p.rapidapi.com/top/anime/1/upcoming",
      headers: {
        "x-rapidapi-key": "d070d378bbmshc8f19ecd0f7796dp11cf3djsn60b74ee1cda7",
        "x-rapidapi-host": "jikan1.p.rapidapi.com"
      }
    }).then(result => {
      this.animelist = result.data;
    });
  }
};
</script>
