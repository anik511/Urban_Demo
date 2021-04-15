<template>
  <div id="app">
    <NavBar />
    <router-view />
    <Footer />
  </div>
</template>

<script>
import NavBar from "@/components/NavBar";
import Footer from "@/components/Footer.vue";
export default {
  components: {
    NavBar,
    Footer,
  },
};
</script>

<style>
/* vendors css */
@import "./assets/vendors/css/grid.css";
@import "./assets/vendors/css/normalize.css";
/* vendors css */
/* fonts */
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600;700&family=Playfair+Display:wght@400;500;600;700&display=swap");
/* fonts */
* {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
  scroll-behavior: smooth;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
ul li {
  list-style-type: none;
}

a {
  text-decoration: none;
}
i {
  color: black;
}
h1 {
  font-size: 4.2rem;
}
body {
  /* font-family: "Open Sans", sans-serif; */
  font-family: "Playfair Display", serif;
  text-rendering: optimizeLegibility;
}
.row {
  max-width: 140rem;
  margin: 0 auto;
}
.main-container {
  padding-bottom: 0;
  margin-top: 0rem;
  padding: 3.5rem 3.8rem;
}
</style>
