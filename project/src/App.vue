<template>
  <div id="app">
    <Navbar/>
    <router-view/>
    <Footer/>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
import Footer from "@/components/Footer";

export default {
  Name: "app",
  components: {
    Navbar,
    Footer
  }
};
</script>


<style lang="scss">
$primaryColor: #4384a1;
$secondaryColor: #86bcda;
$callToActionColor: #ffc551;
$break-small: 640px;
$break-large: 1920px;

/* RESET BASICS */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
/* END OF RESET SECTION */

.wrapper {
  display: flex;
  flex-flow: column wrap;
  height: 100%;
  align-items: flex-start;
}

.row {
  display: inline-flex;
  flex-flow: row wrap;
  /* Then we define how is distributed the remaining space */
  height: 100%;
}

.col {
  flex-flow: column wrap;
  /* Then we define how is distributed the remaining space */
  justify-content: space-around;
}

.justify-content-between {
  justify-content: space-between;
}

/* Buttons */
.btn {
  border-radius: 2px;
  padding: 0.5rem;
  border-width: 0;
  outline: none;
  border-radius: 2px;
  box-shadow: 0 1px 4px rgba(0, 0, 0, 0.6);
  transition: background-color 0.3s;
}

.btn-primary {
  background: $primaryColor;
  &:hover,
  &:active {
    background: $secondaryColor;
  }
}
.btn-secondary {
  background: $secondaryColor;
  &:hover,
  &:active {
    background: $primaryColor;
  }
}

.btn-cta {
  background: $callToActionColor;
  padding: 1rem;
  &:hover,
  &:active {
    background: $secondaryColor;
  }
}

/* End of Buttons Section */
</style>
