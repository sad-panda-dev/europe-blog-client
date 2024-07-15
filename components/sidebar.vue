<template>
    <div class="w-80 p-4 bg-gray-100">
      <div class="mb-8">
        <h3 class="text-lg font-semibold mb-4">Follow Me</h3>
        <div class="flex space-x-4 text-2xl text-gray-600">
          <a href="https://x.com/pudd1ejump3r"><i class="fab fa-twitter"></i></a>
          <a href="https://instagram.com"><i class="fab fa-instagram"></i></a>
        </div>
      </div>
      <div class="mb-8">
        <h3 class="text-lg font-semibold mb-4">Latest</h3>
        <div class="space-y-4">
          <div class="flex items-center" v-for="post in latestPosts" :key="post.id">
            <img :src="post.image" alt="Post Image" class="w-10 h-10 mr-4 rounded-full">
            <a :href="post.link" class="text-sm">{{ post.title }}</a>
          </div>
        </div>
      </div>
      <div class="mb-8">
        <h3 class="text-lg font-semibold mb-4">Categories</h3>
        <div class="grid grid-cols-2 gap-2">
          <div v-for="category in categories" :key="category.name" class="text-center">
            <img :src="category.image" alt="Category Image" class="w-full h-20 object-cover rounded-md mb-2">
            <a :href="category.link" class="text-sm">{{ category.name }}</a>
          </div>
        </div>
      </div>
      <div>
        <h3 class="text-lg font-semibold mb-4">Popular</h3>
        <div class="space-y-4">
          <div class="flex items-center" v-for="post in popularPosts" :key="post.id">
            <img :src="post.image" alt="Post Image" class="w-10 h-10 mr-4 rounded-full">
            <a :href="post.link" class="text-sm">{{ post.title }}</a>
          </div>
        </div>
      </div>
    </div>
</template>
  
<script>
  import asiaPhoto from '@/assets/kalle-kortelainen-6F-uGWod7Xk-unsplash.jpg';
  import europePhoto from '@/assets/david-kohler-VFRTXGw1VjU-unsplash.jpg';
  import naPhoto from '@/assets/bronson-valley-vJnEroC1NuQ-unsplash.jpg';
  import squintingPanda from '@/assets/squinting.png';
  export default {
    data() {
      return {
        latestPosts: [
          { id: 1, title: "Placeholder for latest post #1", image: squintingPanda, link: "#" },
          { id: 2, title: "Placeholder for latest post #2", image: squintingPanda, link: "#" },
          { id: 3, title: "Placeholder for latest post #3", image: squintingPanda, link: "#" },
          { id: 4, title: "Placeholder for latest post #4", image: squintingPanda, link: "#" }
        ],
        categories: [
          { name: "Asia", image: asiaPhoto, link: "#" },
          { name: "Europe", image: europePhoto, link: "#" },
          { name: "North America", image: naPhoto, link: "#" }
        ],
        popularPosts: [
          { id: 1, title: "Placeholder for popular post #1", image: squintingPanda, link: "#" },
          { id: 2, title: "Placeholder for popular post #2", image: squintingPanda, link: "#" },
          { id: 3, title: "Placeholder for popular post #3", image: squintingPanda, link: "#" },
          { id: 4, title: "Placeholder for popular post #4", image: squintingPanda, link: "#" }
        ]
      }
    }
  }
</script>
  
<style scoped>
  .sidebar {
    width: 300px;
    padding: 20px;
    background-color: #f9f9f9;
  }
  .sidebar-section {
    margin-bottom: 20px;
  }
  h3 {
    font-size: 18px;
    margin-bottom: 10px;
  }
  .social-links a {
    margin-right: 10px;
    font-size: 24px;
    color: #333;
  }
  .latest-posts .post,
  .popular-posts .post {
    display: flex;
    align-items: center;
    margin-bottom: 10px;
  }
  .latest-posts .post img,
  .popular-posts .post img {
    width: 40px;
    height: 40px;
    margin-right: 10px;
  }
  .categories .category {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 10px;
  }
  .categories .category img {
    width: 100%;
    height: auto;
  }
</style>
  