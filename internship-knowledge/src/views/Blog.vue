<template>
  <v-container>
    <v-row>
      <v-col cols="12" sm="2">
        <v-sheet rounded="lg" min-height="268">
          Hello
        </v-sheet>
      </v-col>

      <v-col cols="12" sm="8">
        <v-sheet min-height="70vh" rounded="lg">
          Middle
        </v-sheet>
      </v-col>

      <v-col cols="12" sm="2">
        <v-sheet rounded="lg" min-height="268">
          end
        </v-sheet>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  import BlogPostShort from "../components/BlogPostShort";
  import BlogPostFull from "../components/BlogPostFull";

  export default {
    components: {
      BlogPostShort,
      BlogPostFull,
    },
  };
</script>

<style></style>
