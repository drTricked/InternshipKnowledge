<template>
  <!-- take out app prop if you don't want it to stick -->
  <v-app-bar app dense color="primary" dark>
    <div class="d-flex align-center">
      <v-btn text>
        <router-link class="r-link" to="/">Home</router-link>
      </v-btn>
      <v-btn text>
        <router-link class="r-link" to="/About">About</router-link>
      </v-btn>
      <v-btn text>
        <router-link class="r-link" to="/Blog">Blog</router-link>
      </v-btn>
    </div>

    <v-spacer></v-spacer>

    <v-btn
      href="https://github.com/vuetifyjs/vuetify/releases/latest"
      target="_blank"
      text
    >
      <span class="mr-2">Latest Release</span>
      <v-icon>mdi-open-in-new</v-icon>
    </v-btn>
  </v-app-bar>
</template>

<script>
  export default {};
</script>

<style lang="scss" scoped>
  .r-link {
    color: white;
    text-decoration: none;
  }
</style>
