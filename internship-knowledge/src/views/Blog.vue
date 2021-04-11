<template>
  <v-container>
    <v-row>
      <v-col cols="12" sm="1">
        <v-sheet rounded="lg" min-height="268">
          Hello
        </v-sheet>
      </v-col>

      <v-col cols="12" sm="9">
        <v-sheet min-height="70vh" rounded="lg">
          <BlogPostFull
            v-for="(post, index) in posts"
            :key="index"
            :title="post.title"
            :date="post.date"
            :text="post.text"
          />
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
  //   import BlogPostShort from "../components/BlogPostShort";
  import BlogPostFull from "../components/BlogPostFull";

  export default {
    components: {
      //  BlogPostShort,
      BlogPostFull,
    },
    data: () => ({
      posts: [
        {
          title: "First Blog Post!",
          date: new Date(),
          text: "This is my first blog post!!!",
        },
        {
          title: "Second Blog Post!",
          date: new Date(),
          text: "Second blog post, lets gooooo!!!",
        },
      ],
    }),
  };
</script>

<style></style>
