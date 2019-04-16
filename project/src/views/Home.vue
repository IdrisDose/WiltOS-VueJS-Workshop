<template>
  <div class="wrapper">
    <Banner/>
    <Articles v-bind:articles="posts"/>
  </div>
</template>

<script>
//@ is the same as ..
import Banner from "@/components/Banner";
import Articles from "@/components/articles/Index";
import posts from "@/assets/posts.json";
import axios from "axios";

export default {
  components: {
    Banner,
    Articles
  },
  data() {
    return {
      posts
    };
  }
};
</script>

