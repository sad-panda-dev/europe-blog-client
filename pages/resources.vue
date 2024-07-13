<template>
    <NavBar />
    <div>
        <h1>Resources</h1>
    </div>
    <FooterLite />
</template>
<script lang="ts">
import { defineComponent } from 'vue';
  import NavBar from '../components/navBar.vue';
  import footerLite from '~/components/footerLite.vue';
import FooterLite from '~/components/footerLite.vue';
  
  export default defineComponent({
    name: 'ResourcesPage',
    components: {
      NavBar,
      FooterLite
    }
  });
</script>
<style scoped>
    
</style>