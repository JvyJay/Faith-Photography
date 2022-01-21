<template>
  <div id="app">
    <Navbar v-bind:img="img" v-bind:alt="alt" />
  </div>
</template>

<script>
// Logo Image
import img from "./assets/logo.png";
  import Navbar from "./components/Navbar.vue";

export default {
  components: {
    Navbar
  },
  data() {
    return {
        img: img,
        alt: "Logo"
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

h1 {
  margin-bottom: 50px;
  margin-top: 50px;
}

.footer {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.btn {
  color: rgb(255, 149, 220);
  border-color: rgb(255, 149, 220);
}

.btn-secondary {
  color: rgb(255, 149, 220);
  background-color: #fff;
  border-color: rgb(255, 149, 220);
}

.btn:hover {
    color: #fff;
    background-color: rgb(255, 149, 220);
    transition: ease-in-out 0.1s;
}
</style>
