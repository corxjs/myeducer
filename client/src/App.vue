<template>
  <v-app>
    <v-app-bar app color="grey darken-3" dark>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          :src="require('./assets/logo2.svg')"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          :src="require('./assets/logo.svg')"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn text>
        <span class="mr-1">Login</span>
      </v-btn>
      <v-divider vertical></v-divider>
      <v-btn class="mr-2" text>
        <span class="mr-1">Join</span>
        <v-icon>mdi-leaf</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <Home />
    </v-main>
  </v-app>
</template>

<script>
import Home from "./components/Home";
export default {
  name: "App",
  data() {
    return {};
  },
  components: {
    Home,
  },
  computed: {},
  methods: {},
};
</script>