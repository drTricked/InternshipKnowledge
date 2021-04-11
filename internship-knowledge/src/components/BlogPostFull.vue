<template>
  <v-card flat>
    <v-card-title>{{ title }}</v-card-title>
    <v-card-subtitle
      >{{ date.toDateString() }}
      {{ date.toLocaleTimeString() }}</v-card-subtitle
    >
    <v-card-text>{{ text }}</v-card-text>
  </v-card>
</template>

<script>
  export default {
    props: {
      title: { type: String, default: "" },
      date: { type: Date, default: "" },
      text: { type: String, default: "" },
    },
  };
</script>

<style></style>
