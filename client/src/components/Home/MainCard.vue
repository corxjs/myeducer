<template>
  <v-card class="mx-auto" color="purple" dark max-width="400">
    <v-card-title>
      <img class="icon-logo" left :src="icons.logo" width="40" />
      <span class="overline ml-auto font-weight-bold">MYEDUCER</span>
    </v-card-title>
    <v-card-text class="headline-4 font-weight-bold">
      “In the end we retain from our studies only that which we practically
      apply.” <sub>-Goethe</sub>
    </v-card-text>
    <v-card-actions>
      <v-list-item class="grow">
        <v-text-field
          append-icon="mdi-video"
          label="Search Online Educer"
        ></v-text-field>
      </v-list-item>
    </v-card-actions>
  </v-card>
</template>
<script>
import logo from "../../assets/logo2.svg";
export default {
  data: () => ({
    icons: { logo },
  }),
};
</script>
<style lang="css">
.icon-logo {
  position: relative;
  animation: 0.5s alternate-reverse infinite iconlogo ease;
}
@keyframes iconlogo {
  0% {
    left: 0;
  }

  100% {
    left: 3px;
  }
}
</style>