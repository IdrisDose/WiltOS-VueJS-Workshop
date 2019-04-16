<template>
  <div id="nav">
    <div class="nav-menu">
      <img :src="img" alt>
      <router-link to="/" class="nav-link">Home</router-link>
      <router-link to="/about" class="nav-link">About</router-link>
    </div>
  </div>
</template>

<script>
import img from "@/assets/logo.png";

export default {
  name: "Navbar",
  data() {
    return {
      img
    };
  }
};
</script>

<style lang="scss" scoped>
$primaryColor: #4384a1;
$secondaryColor: #86bcda;
$callToActionColor: #ffc551;

#nav {
  height: 56px;
  line-height: 56px;
  background: $primaryColor;
  display: flex;

  .nav-menu {
    width: 50%;
    margin: 0 auto;
    display: inline-flex;
    align-self: center;
    img {
      width: 50px;
      margin-right: 1rem;
    }
    .nav-link {
      height: 56px;
      margin-left: 0.1rem;
      padding-left: 1rem;
      padding-right: 1rem;
      text-decoration: none;
      color: #f2f2f2;
      cursor: pointer;
      transition: background 0.3s;
      &:hover {
        background: $secondaryColor;
      }
    }
  }
}
</style>

