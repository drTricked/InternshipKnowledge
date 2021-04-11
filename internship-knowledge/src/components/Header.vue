<template>
  <!-- take out app prop if you don't want it to stick -->
  <v-app-bar app flat dense dark color="grey">
    <v-app-bar-title> InternshipKnowledge</v-app-bar-title>
    <v-spacer></v-spacer>
    <div class="d-flex align-center">
      <v-btn text>
        <router-link class="r-link font-weight-light" to="/">Home</router-link>
      </v-btn>
      <v-btn text>
        <router-link class="r-link font-weight-light" to="/about"
          >About</router-link
        >
      </v-btn>
      <v-btn text>
        <router-link class="r-link font-weight-light" to="/blog"
          >Blog</router-link
        >
      </v-btn>
      <v-btn text>
        <router-link class="r-link font-weight-light" to="/goals"
          >Goals</router-link
        >
      </v-btn>
    </div>
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
