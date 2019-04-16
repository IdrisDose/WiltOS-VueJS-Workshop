<template>
  <div class="article">
    <h2>{{ article.title }}</h2>
    <p>{{ article.text }}</p>
  </div>
</template>

<script>
export default {
  Name: "Article",
  props: ["article"],
  created() {
    console.log(this.$props.article);
  }
};
</script>

<style lang="scss" scoped>
.article {
  padding: 1rem;
  margin: 2rem;
  border-radius: 2px;
  box-shadow: 0 1px 4px rgba(0, 0, 0, 0.6);

  //Flex Magic
  flex: 1 1 150px;
}
</style>
