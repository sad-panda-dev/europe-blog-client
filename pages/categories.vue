<template>
    <NavBar />
    <div>
        <h1>Categories</h1>
    </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue';
  import NavBar from '../components/navBar.vue';
  
  export default defineComponent({
    name: 'CategoriesPage',
    components: {
      NavBar
    }
  });
</script>
<style scoped>
    
</style>