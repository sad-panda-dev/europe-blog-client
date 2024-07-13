<template>
    <nav class="navbar">
      <div class="navbar-brand">
        <a class="navbar-item" href="#">
          Puddle Jumping
        </a>
      </div>
      <div class="navbar-menu">
        <div class="navbar-start">
          <nuxt-link class="navbar-item" to="/">About</nuxt-link>
          <nuxt-link class="navbar-item" to="/destinations">Destinations</nuxt-link>
          <nuxt-link class="navbar-item" to="/categories">Categories</nuxt-link>
          <nuxt-link class="navbar-item" to="/resources">Resources</nuxt-link>
          <nuxt-link class="navbar-item" to="/contact">Contact</nuxt-link>
        </div>
        <div class="navbar-end">
          <a class="navbar-item" href="#"><i class="fa-brands fa-twitter"></i></a>
          <a class="navbar-item" href="#"><i class="fa-brands fa-instagram"></i></a>
        </div>
      </div>
    </nav>
</template>
  
<script lang="ts">
  import { defineComponent } from 'vue';
  
  export default defineComponent({
    name: 'NavBar',
  });
</script>
  
<style scoped>
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 2rem;
    background-color: #fff;
    border-bottom: 1px solid #eaeaea;
  }
  
  .navbar-brand .navbar-item {
    font-size: 1.5rem;
    font-weight: bold;
    color: #000;
    text-decoration: none;
  }
  
  .navbar-menu {
    display: flex;
    align-items: center;
  }
  
  .navbar-start .navbar-item,
  .navbar-end .navbar-item {
    margin-right: 1rem;
    color: #000;
    text-decoration: none;
  }
  
  .navbar-start .navbar-item.active,
  .navbar-start .navbar-item:hover {
    border-bottom: 2px solid #00aaff;
  }
  
  .navbar-end .navbar-item i {
    font-size: 1.2rem;
  }
  
  .navbar-end .navbar-item:hover i {
    color: #00aaff;
  }
</style>
  