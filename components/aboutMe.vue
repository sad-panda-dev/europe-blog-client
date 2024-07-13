<template>
    <section class="about-me bg-gray-100 py-10">
      <div class="container mx-auto flex flex-col items-center md:flex-row md:items-center md:space-x-10">
        <div class="w-48 h-48 mb-6 md:mb-0">
          <img src="@/assets/profilePic.jpeg" alt="Profile Picture" class="rounded-full border-4 border-white shadow-md" />
        </div>
        <div class="text-center md:text-left">
          <h2 class="text-2xl font-bold mb-4">Hi! I’m Rick</h2>
          <p class="text-gray-700 mb-4">
            I am a software developer, and an ex chef of over 15 years experience. I enjoy traveling and experiencing different cultures
            food and sights. I share my adventures in hopes to inspire anyone with a similar curiosity and wanderlust.
          </p>
          <a href="#" class="text-blue-500 hover:underline block mb-4">More About Me</a>
          <div class="flex justify-center md:justify-start space-x-4">
            <a href="#" class="text-blue-500 hover:text-blue-700">
              <i class="fab fa-facebook-square fa-2x"></i>
            </a>
            <a href="#" class="text-blue-500 hover:text-blue-700">
              <i class="fab fa-twitter-square fa-2x"></i>
            </a>
            <a href="#" class="text-blue-500 hover:text-blue-700">
              <i class="fab fa-instagram-square fa-2x"></i>
            </a>
          </div>
        </div>
      </div>
    </section>
</template>
  
<script setup lang="ts">
</script>
  
<style scoped>
  .about-me {
    background-color: #f7f7f7;
  }
  
  img {
    width: 100%;
    height: auto;
    object-fit: cover;
  }
</style>
  