<template>
    <div>
        <b-card
        title="About Me"
        v-bind:img-src="img"
        v-bind:img-alt="alt"
        img-top
        style="max-width: 80%"
        class="mb-2 mx-auto"
  >
    <b-card-text>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit voluptate earum corrupti possimus ea nisi recusandae labore ut facere, fuga magnam tenetur tempore quasi voluptas. Illum qui quasi aliquid dolor, pariatur officia quibusdam voluptas cupiditate. Sunt quaerat, iste magnam laudantium minus, modi sit fugit maiores consequatur sapiente dolores voluptatum molestias?
    </b-card-text>

    <b-button pill href="#">Contact</b-button>
  </b-card>
    </div>
</template>

<script>
import Vue from 'vue';

import img from "D:/Web Dev-Design/Portfolio-Projects/faith-photography/src/assets/about-photo.jpeg"

export default Vue.component("AboutCard",{
    name: "AboutCard",
    data() {
        return {
            img: img,
            alt: "About Image"
        }
    }
})
</script>
