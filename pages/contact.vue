<template>
    <NavBar />
    <div>
        <h1>Contact</h1>
    </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue';
  import NavBar from '../components/navBar.vue';
  
  export default defineComponent({
    name: 'ContactPage',
    components: {
      NavBar
    }
  });
</script>
<style scoped>
    
</style>