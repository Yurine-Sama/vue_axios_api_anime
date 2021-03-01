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
      url: "https://jikan1.p.rapidapi.com/top/anime/1/upcoming"
    }).then(result => {
      this.animelist = result.data;
    });
  }
};
</script>
