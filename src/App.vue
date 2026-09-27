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
      <h2 class="text-2xl font-bold text-indigo-custom mb-8 text-center">Projects</h2>
      <ProjectGrid :projects="projectsData" />
    </div>
  </section>

  <section id="about" class="py-16 px-4 bg-gray-50 text-center">
    <div class="max-w-4xl mx-auto">
      <h2 class="section-title text-2xl font-bold text-indigo-custom mb-8">About</h2>

      <div class="grid md:grid-cols-2 gap-8 items-center">
        <div class="space-y-4 text-gray-600">
          <p>I'm Ayaan, a sophomore at <span>NJIT</span> currently pursuing a <span>Math</span> & CS degree with a minor in physics.</p>
          <p>I absolutely love creating. Blah... I like art, writing, video games, but I just like the process of making something.</p>
          <p>Outside of programming I love to write and draw. I've been learning game development and am currently planning on making my own game.</p>
        </div>

        <div class="font-bold text-indigo-custom mb-3">Tech I use</div>
        <div class="flex flex-wrap gap-2">
          <!-- DYNAMICALLY GENERATE A LIST: godot, procreate, vue, vite, tailwind, js, java, python, godot, MATLAB -->
        </div>
      </div>
    </div>
  </section>

  <footer class="py-8 text-center text-gray-500 text-sm">
    <a href="https://github.com/AynAws" class="hover:underline">GitHub</a>
    |
    <a href="mailto:ayaanawais173@gmail.com" class="hover:underline">Email</a>
  </footer>
</template>