<template>
  <div>
    <div>
    <Carousel 
    v-bind:carousel1="carousel1"
    v-bind:carousel2="carousel2"
    v-bind:carousel3="carousel3"
    v-bind:carousel4="carousel4" />
    </div>
    <div>
    <Gallery  />
    </div>
  </div>
</template>

<script>
// Components
import Carousel from '../components/Carousel.vue';
import Gallery from '../components/Gallery.vue';
// Carousel Images
import carousel1 from "../assets/carousel01.jpg";
import carousel2 from "../assets/carousel02.jpg";
import carousel3 from "../assets/carousel03.jpg";
import carousel4 from "../assets/carousel04.jpg";
// Gallery Images
import img1 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/image0.jpeg";
import img2 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/image2.jpeg";
import img3 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/img1.png";
import img4 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/img2.png";
import img5 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/img4.png";
import img6 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/img5.png";
import img7 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/img7.png";
import img8 from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/img/img8.png";


export default {
  name: 'Home',

  components: {
    Carousel,
    Gallery
  },

  data() {
    return {
      carousel1: carousel1,
      carousel2: carousel2,
      carousel3: carousel3,
      carousel4: carousel4,
      images: [
        {
          id: 0,
          title: "Row 1",
          images: [
                    {
                  id: 0,
                  img: img1,
                  alt: "Image 1"
                },
                {
                  id: 1,
                  img: img2,
                  alt: "Image 2"
                },
          ]
        },
        {
          id: 1,
          title: "Row 1",
          images: [
                    {
                  id: 0,
                  img: img3,
                  alt: "Image 3"
                },
                {
                  id: 1,
                  img: img4,
                  alt: "Image 4"
                },
          ]
        },
        {
          id: 2,
          title: "Row 1",
          images: [
                    {
                  id: 0,
                  img: img5,
                  alt: "Image 5"
                },
                {
                  id: 1,
                  img: img6,
                  alt: "Image 6"
                },
          ]
        },
        {
          id: 3,
          title: "Row 1",
          images: [
                    {
                  id: 0,
                  img: img7,
                  alt: "Image 7"
                },
                {
                  id: 1,
                  img: img8,
                  alt: "Image 8"
                },
          ]
        },
      ]
      }
    }
  }
</script>
