<template>
  <div>
    <div class="home-video">
      <video
        ref="homeVideo"
        :src="homevideo"
        style="width: 100vw"
        muted
        loop
        autoplay
      ></video>
    </div>
    <v-container fluid class="card-container">
      <v-row>
        <v-col cols="12" md="6" offset-md="3">
          <MainCard />
        </v-col>
      </v-row>
    </v-container>
    <v-divider class="my-4"></v-divider>
    <v-container fluid class="introduction">
      <v-row>
        <v-col cols="12" md="6">
          <v-img :src="require('../assets/images/home/edu.png')" />
        </v-col>
        <v-col cols="12" md="6">
          <p class="ultra-title">Age is online age</p>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import homevideo from "../assets/videos/home.mp4";
import MainCard from "./Home/MainCard.vue";

export default {
  data() {
    return {
      homevideo,
    };
  },
  components: {
    MainCard,
  },
};
</script>

<style>
.card-container {
  position: absolute;
  top: 9%;
  z-index: 1;
}
.home-video {
  filter: grayscale(40%) sepia(10%) brightness(1) blur(2px);
  height: 38vh;
  margin-bottom: 15vh;
  overflow: hidden;
  vertical-align: center;
}
.introduction {
  height: 100vh;
}
.ultra-title {
  font-size: 7em;
  font-family: fantasy;
}
</style>