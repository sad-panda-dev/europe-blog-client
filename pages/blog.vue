<template>
  <div>
    <NavBar />
    <div class="blog-layout">
      <div class="main-content">
        <h1>Blog</h1>
      </div>
      <SideBar class="sidebar" />
    </div>
    <FooterLite />
  </div>
</template>

<script>
  import NavBar from '../components/navBar.vue';
  import FooterLite from '../components/footerLite.vue';
  import SideBar from '../components/sidebar.vue';

  export default {
      components: {
        NavBar,
        FooterLite,
        SideBar
      }
    };
</script>

<style scoped>
  .blog-layout {
    display: flex;
    justify-content: space-between;
    padding: 16px;
  }

  .main-content {
    flex: 1;
    padding: 16px;
  }

  .sidebar {
    width: 300px;
    padding: 16px;
    background-color: #f9f9f9;
  }
</style>
