<template>
    <NavBar />
    <div>
        <h1>Categories</h1>
    </div>
    <FooterLite />
</template>
<script lang="ts">
import { defineComponent } from 'vue';
  import NavBar from '../components/navBar.vue';
  import FooterLite from '~/components/footerLite.vue';
  
  export default defineComponent({
    name: 'CategoriesPage',
    components: {
      NavBar,
      FooterLite
    }
  });
</script>
<style scoped>
    
</style>