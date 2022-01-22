<template>
  <div class="contact">
      <h1>Contact Me</h1>
        <b-container fluid>
          <p><span>Email:</span> {{ email }}</p>
          <p><span>Phone:</span> {{ phone }}</p>
          <p><span>Instagram:</span> {{ insta }}</p>
          <div class="social-icons">
            <a href="mailto:faithvadnaisphotography@gmail.com"><img width="20px" :src="gmail" alt="Email"></a>
            <a href="https://www.instagram.com/faithvadnaisphotography/"><img width="20px" :src="instagram" alt="Instagram"></a>
          </div>
        </b-container>
      <div class="footer">
        <footer>Copyright © Faith Photography 2022</footer>
      </div>
    </div>
</template>

<script>
// Components
import Footer from "../components/Footer.vue";

// Images
import gmail from "../assets/gmail.png";
import instagram from "../assets/instagram.png";

export default {
  name: 'Contact',

  components: Footer,

  data() {
    return {
      email: "faithvadnaisphotography@gmail.com",
      phone: `+1 (206) 472-9688`,
      insta: "faithvadnaisphotography",
      gmail: gmail,
      instagram: instagram
    }
  }
}
</script>

<style scoped>
  span {
    color: rgb(255, 149, 220);
  }

  footer {
    position: absolute;
    padding: 50px;
    bottom: 0;
  }

  a {
    margin: 10px;
  }
</style>