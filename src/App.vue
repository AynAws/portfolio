<script setup>
import Hero from './components/Hero.vue'
import ProjectGrid from './components/ProjectGrid.vue'
import projectsData from './data/projects.json'
</script>

<template>
  <Hero />

  <section id="projects" class="py-16 px-4 max-w-5xl mx-auto">
    <h2 class="text-2xl font-bold text-gray-900 mb-8 text-center">Projects</h2>
    <ProjectGrid :projects="projectsData" />
  </section>

  <section id="about" class="py-16 px-4 max-w-5xl mx-auto">
    <h2 class="text-2xl font-bold text-gray-900 mb-8 text-center">Projects</h2>
    <ProjectGrid :projects="projectsData" />
  </section>

  <section id="about" class="py-16 px-4 max-w-2xl mx-auto text-center">
    <h2 class="text-2xl font-bold text-gray-900 mb-4">About</h2>
    <p class="text-gray-600">
      Lorem ipsum dolor, sit amet consectetur adipisicing elit. Minus atque corrupti repellat minima.
    </p>
  </section>

  <footer class="py-8 text-center text-gray-500 text-sm">
    <a href="https://github.com/AynAws" class="hover:underline">GitHub</a>
    |
    <a href="mailto:ayaanawais173@gmail.com" class="hover:underline">Email</a>
  </footer>
</template>