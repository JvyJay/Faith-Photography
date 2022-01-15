<template>
  <div>
    <Carousel 
    v-bind:carousel1="carousel1"
    v-bind:carousel2="carousel2"
    v-bind:carousel3="carousel3"
    v-bind:carousel4="carousel4" />
  </div>
</template>

<script>
// Components
import Carousel from '../components/Carousel.vue';
// Carousel Images
import carousel1 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/carousel01.jpg";
import carousel2 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/carousel02.jpg";
import carousel3 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/carousel03.jpg";
import carousel4 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/carousel04.jpg";


export default {
  name: 'Home',

  components: {
    Carousel
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
