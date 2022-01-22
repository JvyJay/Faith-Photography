<template>
  <div class="about">
    <h1>About Me</h1>
    <AboutCard />
    <Footer />
  </div>
</template>

<script>
// Components
import AboutCard from "../components/AboutCard.vue"
import Footer from "../components/Footer.vue";

export default {
  name: "About",
  components: {
    AboutCard,
    Footer
  }
}
</script>

