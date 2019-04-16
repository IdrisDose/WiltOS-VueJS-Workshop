<template>
  <div id="banner" class="banner">
    <div class="banner-content">
      <img :src="img" alt="Logo">
      <h1 class="banner-title">Welcome to the website</h1>
      <p class="banner-text">Some website description</p>
      <button class="btn btn-cta" @click="clicked()">Call to Action!</button>
    </div>
  </div>
</template>

<script>
import img from "@/assets/logo.png";

export default {
  name: "Banner",
  data() {
    return {
      img
    };
  },
  methods: {
    clicked() {
      alert("Clicked! (this is bad practice)");
    }
  }
};
</script>

<style lang="scss" scoped>
#banner {
  width: 100%;
  height: 50vh;
  background: #4556b0;

  .banner-content {
    padding: 2rem;
    height: 100%;
    margin: 0 auto;
    text-align: center;
    color: #f2f2f2;

    /* Flex magic*/
    display: flex;
    justify-content: center;
    flex-direction: column;
    text-align: center;

    button {
      margin-top: 2rem;
      width: 175px;
      align-self: center;
    }
    img {
      align-self: center;
      max-width: 10%;
      height: auto;
    }
  }
}
</style>

