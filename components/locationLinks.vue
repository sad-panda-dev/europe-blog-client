<template>
    <section class="location-links bg-gray-100 py-10">
      <div class="container mx-auto grid grid-cols-1 md:grid-cols-3 gap-6 mr-150 ml-150">
        <div v-for="(location, index) in locations" :key="index" class="relative group">
          <img :src="location.image" alt="Location" class="w-full h-48 object-cover rounded-md shadow-md" />
          <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity">
            <a :href="location.link" class="text-white text-lg font-bold">{{ location.name }}</a>
          </div>
        </div>
      </div>
    </section>
</template>
  
<script setup lang="ts">
    import asiaPhoto from '@/assets/kalle-kortelainen-6F-uGWod7Xk-unsplash.jpg';
    import europePhoto from '@/assets/david-kohler-VFRTXGw1VjU-unsplash.jpg';
    import naPhoto from '@/assets/bronson-valley-vJnEroC1NuQ-unsplash.jpg';

  const locations = [
    { name: 'ASIA', image: asiaPhoto, link: '#' },
    { name: 'EUROPE', image: europePhoto, link: '#' },
    { name: 'NORTH AMERICA', image: naPhoto, link: '#' },
  ];
</script>
  
<style scoped>
  .location-links {
    background-color: #f7f7f7;
  }
  
  .group:hover .overlay {
    opacity: 1;
  }
  
  .overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.5);
    display: flex;
    justify-content: center;
    align-items: center;
    opacity: 0;
    transition: opacity 0.3s ease-in-out;
  }
  
  a {
    color: white;
    text-decoration: none;
    font-size: 1.25rem;
  }
</style>
  