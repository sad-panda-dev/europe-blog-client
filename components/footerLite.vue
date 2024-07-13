<template>
    <footer class="relative bg-black text-white py-10">
      <div class="container mx-auto relative z-10 relative bg-black text-white py-10">
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
    </footer>
</template>
  
<script setup lang="ts">
  
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
</style>
  