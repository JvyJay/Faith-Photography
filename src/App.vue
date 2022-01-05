<template>
  <div id="app">
    <Navbar v-bind:img="imageData.img" v-bind:alt="imageData.alt" />
  </div>
</template>

<script>
// Logo Image
import img from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/Logo.png";
  import Navbar from "./components/Navbar.vue";

export default {
  components: {
    Navbar
  },
  data() {
    return {
      imageData:
      {
        img: img,
        alt: "Logo"
      }
    }
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;300&display=swap');

#app {
  font-family: 'Montserrat', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

a {
  text-decoration: none;
  color: #000;
}

a:hover {
  color: rgb(255, 149, 220);
  transition: ease-in-out 0.1s;
}
</style>
