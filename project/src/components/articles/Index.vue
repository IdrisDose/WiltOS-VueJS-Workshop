<template>
  <div id="articles" class="row">
    <Article
      v-bind:article="article"
      v-for="article in articles"
      v-bind:key="article.id"
      class="col"
    />
  </div>
</template>

<script>
import Article from "./Article";
export default {
  name: "Articles",
  components: {
    Article
  },
  props: ["articles"]
};
</script>

<style lang="scss" scoped>
#articles {
}
</style>
