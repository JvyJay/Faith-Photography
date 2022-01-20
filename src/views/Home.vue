<template>
  <div>
    <Carousel 
    v-bind:carousel1="carousel1"
    v-bind:carousel2="carousel2"
    v-bind:carousel3="carousel3"
    v-bind:carousel4="carousel4" />
    <h1>Gallery</h1>
    <Gallery />
    <Footer />
  </div>
</template>

<script>
// Components
import Carousel from '../components/Carousel.vue';
import Gallery from '../components/Gallery.vue';
import Footer from '../components/Footer.vue';
// Carousel Images
import carousel1 from "../assets/carousel01.jpg";
import carousel2 from "../assets/carousel02.jpg";
import carousel3 from "../assets/carousel03.jpg";
import carousel4 from "../assets/carousel04.jpg";


export default {
  name: 'Home',

  components: {
    Carousel,
    Gallery,
    Footer
  },

  data() {
    return {
      carousel1: carousel1,
      carousel2: carousel2,
      carousel3: carousel3,
      carousel4: carousel4
      }
    }
  }
</script>

<style scoped>
h1 {
  margin-bottom: 100px;
}
</style>
