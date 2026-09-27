<script setup>
import ProjectGrid from './components/ProjectGrid.vue'
import projectsData from './data/projects.json'
</script>

<template>
  <section class="hero-fade min-h-screen flex flex-col items-center justify-center text-center px-4 bg-fixed bg-cover">
      <h1 class="text-3xl md:text-5xl font-bold text-gray-900">Ayaan Awais</h1>
      <p class="text-xl text-gray-600 mt-4">A Passionate Web Developer</p>
      <a href="#projects" class="mt-8 px-6 py-3 bg-blue-600 text-white rounded-lg font-medium hover:bg-blue-700 transition-colors">View my work</a>
  </section>

  <section id="projects" class="py-16 px-4 bg-gray-50">
    <div class="max-w-5xl mx-auto">
      <h2 class="text-2xl font-bold text-gray-900 mb-8 text-center">Projects</h2>
      <ProjectGrid :projects="projectsData" />
    </div>

  </section>

  <section id="about" class="py-16 px-4 bg-gray-50 text-center">
    <div class="max-w-4xl mx-auto">
      <h2 class="section-title text-2xl font-bold text-gray-900 mb-4">About</h2>
      <p class="text-gray-600">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Minus atque corrupti repellat minima.
      </p>
    </div>

  </section>

  <footer class="py-8 text-center text-gray-500 text-sm">
    <a href="https://github.com/AynAws" class="hover:underline">GitHub</a>
    |
    <a href="mailto:ayaanawais173@gmail.com" class="hover:underline">Email</a>
  </footer>
</template>