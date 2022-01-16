<template>
<div>
  <b-carousel
    id="carousel-fade"
    style="text-shadow: 0px 0px 2px #000"
    fade
    indicators
  >
    <b-carousel-slide
      :img-src="carousel1"
      class="carousel-img"
    ></b-carousel-slide>
    <b-carousel-slide
      :img-src="carousel2"
      class="carousel-img"
    ></b-carousel-slide>
    <b-carousel-slide
      :img-src="carousel3"
      class="carousel-img"
    ></b-carousel-slide>
    <b-carousel-slide
      :img-src="carousel4"
      class="carousel-img"
    ></b-carousel-slide>
    </b-carousel>
</div>
</template>

<script>
import Vue from "vue";

export default Vue.component("Carousel", {
    props: {
        carousel1: String,
        carousel2: String,
        carousel3: String,
        carousel4: String,
    }
})
</script>

<style scoped>
.carousel-img {
  height: 75vh !important;
}
</style>