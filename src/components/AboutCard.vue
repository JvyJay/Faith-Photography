<template>
    <div>
        <b-card
        title="About Me"
        v-bind:img-src="img"
        v-bind:img-alt="alt"
        img-top
        style="max-width: 50%"
        class="mb-2 mx-auto"
  >
    <b-card-text>
      {{ paragraph }}
    </b-card-text>

    <router-link to="/contact"><b-button pill>Contact</b-button></router-link>
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
            alt: "About Image",
            paragraph: "Let me tell you a little bit about myself! I was born in Port Angeles Washington, a city surrounded by an ocean breeze and evergreen trees. Ever since I was a little girl I’ve always loved nature, water and art. When I got older and moved to the Seattle area I explored my creativity and became passionate in painting and photography. I first started my photography journey to capture my daughter’s childhood, our family’s memories and milestones but quickly realized I wanted to branch out, push myself to shoot in different ways with more people, and challenge myself to do better and learn more about being behind the camera. I’ve been in love with photography ever since! There is something so special about being able to capture a moment in time that you can hold onto and pass down to generations to come and I’d love to capture and create something amazing with you!"
        }
    }
})
</script>

<style scoped>
p {
  margin-bottom: 10px;
}
</style>
