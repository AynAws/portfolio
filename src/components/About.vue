<script setup>
import techData from '../data/tech.json'
import TechPill from './TechPill.vue'
import Term from './Term.vue'
</script>

<template>
  <div class="grid md:grid-cols-2 gap-8 items-center">
    <div class="space-y-4 text-gray-600">
      <p>I'm Ayaan, a sophomore at <Term full="New Jersey Institute of Technology" link="https://www.njit.edu/">NJIT</Term> currently pursuing a <Term full="Computational Mathematics">Math</Term> & CS degree with a minor in physics.</p>
      <p>I absolutely love creating. The reason I enjoy programming is because I can create whatever I want with the time and knowledge.</p>
      <p>Outside of programming I love to write and draw. I've been learning game development and am currently planning on making my own game.</p>
    </div>
  </div>
  <div class="grid md:grid-cols-2 gap-8 items-center">
    <div class="font-bold text-indigo-custom mb-3">Tech I use</div>
    <div class="flex flex-wrap gap-2">
      <TechPill v-for="tech in techData" :key="tech.name" :tech="tech" />
    </div>
  </div>
</template>