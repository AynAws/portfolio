<script setup>
import ProjectCard from './ProjectCard.vue'
defineProps(['projects'])
</script>

<template>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <ProjectCard
          v-for="p in projects"
          :key="p.title"
          :project="p"
        />
    </div>
</template>