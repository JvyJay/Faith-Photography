<template>
  <div class="contact">
    <h1>Contact Me</h1>
    <div class="contact-container">
      <p><span>Email:</span> {{ email }}</p>
      <p><span>Phone:</span> {{ phone }}</p>
      <p><span>Instagram:</span> {{ insta }}</p>
    </div>
    <footer>Copyright © Faith Photography 2022</footer>
  </div>
</template>

<script>
// Components
import Footer from "../components/Footer.vue";

export default {
  name: 'Contact',

  components: Footer,

  data() {
    return {
      email: "somethingsomething@gmail.com",
      phone: `+1 (253) 808-5674`,
      insta: "faithyguzzy666"
    }
  }
}
</script>

<style scoped>
.contact {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

  span {
    color: rgb(255, 149, 220);
  }

  footer {
    position: absolute;
    padding: 50px;
    bottom: 0;
  }
</style>