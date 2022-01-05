<template>
  <div id="app">
    <div>
  <b-navbar toggleable="lg" type="light" variant="light">
    <b-navbar-brand href="#"><img width="300px" src="..\img\Logo.png"></b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav class="ml-auto">
      <!-- <b-navbar-nav>
        <b-nav-item href="#"><router-link to="/">Home</router-link></b-nav-item>
        <b-nav-item href="#"><router-link to="/about">About</router-link></b-nav-item>
        <b-nav-item href="#"><router-link to="/contact">Contact</router-link></b-nav-item>
        <b-nav-item href="#"><router-link to="/services">Services</router-link></b-nav-item>
      </b-navbar-nav> -->

      <!-- Right aligned nav items -->
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

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

a {
  text-decoration: none;
  color: #000;
}
</style>
