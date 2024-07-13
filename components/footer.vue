<template>
    <footer class="relative bg-black text-white py-10">
      <div class="container mx-auto relative z-10">
        <div class="text-center mb-10">
          <h2 class="text-xl font-bold mb-6 text-black">Follow me on Instagram <a class="insta-link" href="#"><i class="fa-brands fa-instagram"></i></a></h2>
          
          <div class="flex flex-wrap justify-center">
            <div
              class="relative m-2 transform translate-y-0"
              :class="{ 'translate-y-4': index % 2 === 1 }"
              v-for="(photo, index) in photos"
              :key="index"
            >
              <div class="polaroid">
                <img :src="photo" alt="Instagram Photo" class="object-cover w-32 h-32" />
              </div>
            </div>
          </div>
        </div>
        <div class="border-t border-gray-700 pt-6 bg-black">
          <div class="flex justify-between items-center">
            <div>
              <p class="text-lg font-bold">Puddle Jumping</p>
            </div>
            <div class="flex space-x-4">
              <NuxtLink to="/moreAboutMe" class="text-white hover:underline block mb-4">About Me</NuxtLink>
              <NuxtLink to="/blog" class="text-white hover:underline block mb-4">Blog</NuxtLink>
              <NuxtLink to="/videos" class="text-white hover:underline block mb-4">Videos</NuxtLink>
              <NuxtLink to="/contact" class="text-white hover:underline block mb-4">Contact</NuxtLink>
              <NuxtLink to="/donate" class="text-white hover:underline block mb-4">Donate</NuxtLink>
            </div>
            <div class="flex space-x-4">
              <a href="https://x.com/pudd1ejump3r"><i class="fa-brands fa-twitter fa-2x"></i></a>
              <a href="#"><i class="fa-brands fa-instagram fa-2x"></i></a>
            </div>
          </div>
        </div>
      </div>
      <div class="absolute inset-0 h-1/2 bg-white z-0"></div>
    </footer>
</template>
  
<script setup lang="ts">
  import photo1 from '@/assets/peter-james-eisenhaure-k6R0EAE4wI4-unsplash.jpg';
  import photo2 from '@/assets/sergey-pesterev-dstd4DoLQ90-unsplash.jpg';
  import photo3 from '@/assets/henry-be-IicyiaPYGGI-unsplash.jpg';
  import photo4 from '@/assets/henrique-craveiro-ezJhm4xrHAM-unsplash.jpg';
  import photo5 from '@/assets/brianna-parks-_glgclBJq5M-unsplash.jpg';
  
  const photos = [photo1, photo2, photo3, photo4, photo5];
</script>
  
<style scoped>
  footer::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 50%;
    background-color: #f7f7f7;
    z-index: -1;
  }

  .insta-link {
    margin-right: 1rem;
    color: #000;
    text-decoration: none;
  }
  
  .polaroid {
    background-color: white;
    padding: 7px 7px 25px 7px;
    display: inline-block;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
  }
  
  .polaroid img {
    display: block;
    max-width: 100%;
    height: auto;
  }
</style>
  