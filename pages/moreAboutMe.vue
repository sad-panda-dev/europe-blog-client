<template>
    <NavBar />
    <div>
        <h1>MoreAboutME</h1>
    </div>
    <FooterLite />
</template>
<script lang="ts">
import { defineComponent } from 'vue';
  import NavBar from '../components/navBar.vue';
  import FooterLite from '../components/footerLite.vue';
  
  export default defineComponent({
    name: 'MoreAboutMePage',
    components: {
      NavBar,
      FooterLite
    }
  });
</script>
<style scoped>
    
</style>