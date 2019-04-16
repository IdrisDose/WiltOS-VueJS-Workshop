<template>
  <div id="footer" class="footer">
    <div class="footer-content">
      <p>&copy; somewebsite 2019</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  components: {}
};
</script>

<style lang="scss" scoped>
#footer {
  position: fixed;
  bottom: 0;
  width: 100%;
  height: 5vh;
  background: #4556b0;

  .footer-content {
    margin: 0 auto;
    text-align: center;
    color: #f2f2f2;
    line-height: 200%;
  }
}
</style>

