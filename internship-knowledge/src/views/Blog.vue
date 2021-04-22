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
          date: new Date("2021-04-11"),
          text: "This is my first blog post!!!",
        },
        {
          title: "Second Blog Post!",
          date: new Date("2021-04-11"),
          text: "Second blog post, lets gooooo!!!",
        },
        {
          title: "April 20 Update",
          date: new Date("2021-04-21 8:00:00"),
          text:
            "Been a couple days since I worked on this website. I have done some practice with Java spring recently, I wanted to get familiar with the technology before hand." +
            " Java spring allows you to write the backend using java. From what I have heard JDBC isn't very nice to work with; interestingly we used it in our databases class." +
            " Not too sure what I should be working on right now. I want to start working on some front end stuff, but there is always more backend to learn." +
            " Ideally I should be starting to work on something that combines all of my knowledge together.",
        },
        {
          title: "April 20 Update pt2",
          date: new Date("2021-04-21 9:00:00"),
          text:
            "Recap: tried using Vue.js, and Java spring. Starting to attempt some blockchain sounds very interesting? Maybe going back and working on a MERN stack would be good." +
            " I am unsure of working on backend with Java so far? Hard to find resources for a Vuejs + Java Spring stack. Plus I still enjoy working on design.",
        },
        {
          title: "April 21 Update",
          date: new Date("2021-04-21 11:04:00"),
          text:
            "Future plans: work on front end designs of portfolio site, start deploying to github pages, work on a bucket list and travel website, update this so this can be done through a model on the website and link this to a backend.",
        },
        {
          title: "April 21 Update pt2",
          date: new Date("2021-04-21 20:05:00"),
          text:
            "Followed a tutorial to create a Exercise Tracker using the MERN stack.",
        },
      ],
    }),
  };
</script>

<style></style>
