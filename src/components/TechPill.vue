<script setup>
defineProps(['tech'])
</script>

<template>
  <a
    :href="tech.link"
    target="_blank"
    rel="noopener"
    class="flex items-center gap-2 text-xs px-3 py-1.5 rounded-full font-medium transition-transform hover:scale-105"
    :style="{ backgroundColor: tech.color + '20', color: tech.color }"
  >
    <img :src="tech.img" :alt="tech.alt" class="w-4 h-4" />
    {{ tech.name }}
  </a>
</template>