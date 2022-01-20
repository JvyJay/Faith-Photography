<template>
  <div>
    <div>
  <b-navbar toggleable="lg" type="light" variant="light">
    <b-navbar-brand href="#"><img width="200px" :src="img" alt="alt"></b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav class="ml-auto">
      <b-navbar-nav class="ml-auto" right>
        <b-nav-item href="#"><router-link to="/">Home</router-link></b-nav-item>
        <b-nav-item href="#"><router-link to="/about">About</router-link></b-nav-item>
        <b-nav-item href="#"><router-link to="/contact">Contact</router-link></b-nav-item>
        <b-nav-item href="#"><router-link to="/services">Services</router-link></b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
    <router-view/>
  </div>
</template>

<script>
import Vue from "vue";

export default Vue.component("Navbar", {
    props: {
        img: String,
        alt: String
    }
})
</script>