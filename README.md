<template>
  <div class="bg-blue-900 text-white min-h-screen flex flex-col items-center justify-center space-y-8">
    <!-- Hero Section -->
    <div class="text-center">
      <h1 class="text-5xl font-bold mb-4 animate__animated animate__fadeIn">Hi.. I'm Hawaaan!</h1>
      <img
        src="your-avatar.jpg" 
        alt="Hawaaan's Avatar"
        class="w-32 h-32 rounded-full mx-auto shadow-lg transform transition duration-500 hover:scale-110"
      />
    </div>

    <!-- About Me Section -->
    <div class="text-center">
      <h2 class="text-3xl font-semibold mb-2 animate__animated animate__fadeIn">About Me</h2>
      <p class="max-w-xl mx-auto text-lg mb-6 animate__animated animate__fadeIn">
        I'm a passionate Full Stack Developer with expertise in Vue 3, TypeScript, and Tailwind CSS.
      </p>
    </div>

    <!-- Tech Stack Section -->
    <div class="flex space-x-6 justify-center animate__animated animate__fadeIn">
      <img src="vue-icon.svg" alt="Vue.js" class="w-12 h-12 hover:animate-pulse" />
      <img src="typescript-icon.svg" alt="TypeScript" class="w-12 h-12 hover:animate-pulse" />
      <img src="tailwind-icon.svg" alt="Tailwind CSS" class="w-12 h-12 hover:animate-pulse" />
    </div>

    <!-- Projects Section -->
    <div class="text-center mt-8">
      <h2 class="text-3xl font-semibold mb-4">Projects</h2>
      <ul class="space-y-4">
        <li class="animate__animated animate__fadeIn">
          <a href="https://cirfeed.com" class="text-xl font-medium text-blue-400 hover:text-blue-500">
            Cirfeed - Tech News Platform
          </a>
        </li>
        <li class="animate__animated animate__fadeIn">
          <a href="https://github.com/Hawaaan/portfolio" class="text-xl font-medium text-blue-400 hover:text-blue-500">
            Portfolio - Personal Website
          </a>
        </li>
        <li class="animate__animated animate__fadeIn">
          <a href="https://github.com/Hawaaan/vue-alerts" class="text-xl font-medium text-blue-400 hover:text-blue-500">
            Vue Alerts - Reusable Vue 3 Component
          </a>
        </li>
      </ul>
    </div>

    <!-- Contact Section -->
    <div class="flex space-x-6 mt-8">
      <a href="https://linkedin.com/in/eng-zoja" class="text-blue-600 hover:text-blue-800">
        <img src="linkedin-icon.svg" alt="LinkedIn" class="w-10 h-10" />
      </a>
      <a href="https://twitter.com/yourtwitter" class="text-blue-400 hover:text-blue-600">
        <img src="twitter-icon.svg" alt="Twitter" class="w-10 h-10" />
      </a>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: 'Profile',
};
</script>

<style scoped>
/* Add custom animations */
@import 'animate.css';

.text-5xl {
  animation: fadeIn 1s ease-out;
}
</style>
