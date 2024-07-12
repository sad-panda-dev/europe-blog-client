<template>
    <div>
      <NavBar />
      <!-- Rest of your content goes here -->
      <section>
        <!-- Example of main content -->
        <div class="main-content">
          <img src="../assets/micael-rodrigues-G3XXUyKYmHo-unsplash.jpg" alt="Navigating Mountains In Durmitor National Park" class="hero-image">
          <div class="overlay">
            <h2>Navigating Mountains In Durmitor National Park</h2>
            <p>When we showed up in Montenegro, a country that literally translates as "Black Mountain," we were determined to spend some time exploring the peaks and crags around the place.</p>
            <a class="btn" href="#">Read</a>
          </div>
        </div>
      </section>
    </div>
  </template>
  
  <script lang="ts">
  import { defineComponent } from 'vue';
  import NavBar from '../components/navBar.vue';
  
  export default defineComponent({
    name: 'IndexPage',
    components: {
      NavBar
    }
  });
  </script>
  
  <style scoped>
  .main-content {
    position: relative;
    text-align: center;
    color: white;
  }
  
  .hero-image {
    width: 100%;
    height: auto;
  }
  
  .overlay {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background: rgba(0, 0, 0, 0.5);
    padding: 20px;
    border-radius: 10px;
  }
  
  .btn {
    display: inline-block;
    padding: 10px 20px;
    background-color: #00aaff;
    color: #fff;
    text-decoration: none;
    border-radius: 5px;
    margin-top: 10px;
  }
  
  .btn:hover {
    background-color: #0088cc;
  }
  </style>
  