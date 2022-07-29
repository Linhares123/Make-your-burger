<template>
  <Navbar :logo="logo_src" :alt="app_name" />
  <RouterView />
  <Footer1 />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Footer1 from "./components/Footer.vue";

export default {
  components: {
    Navbar,
    Footer1,
  },

  data() {
    return {
      logo_src: "/img/logo.png",
      app_name: "Make Your Burguer",
    };
  },
};
</script>

<style>
* {
  box-sizing: border-box;

  font-family: Helvetica;

  padding: 0;
  margin: 0;
}

.main-container {
  margin: 50px;
  min-height: 250px;
}

h1 {
  text-align: center;
  font-size: 42px;

  color: #222;

  margin-bottom: 30px;
}
</style>
