<script setup>
defineProps(['project'])
</script>

<template>
    <div class="rounded-xl bg-white shadow-md overflow-hidden flex flex-col">
        <img :src="project.image" :alt="project.alt" class="w-full h-40 object cover">

        <div class="p-5 flex flex-col flex-1">
            <h3 class="text-lg font-bold text-gray-900">{{ project.title }}</h3>
            <p class="text-gray-600 text-sm mt-2 flex-1">{{ project.desc }}</p>

            <div class="flex flex-wrap mt-2 mt-4">
                <span
                  v-for="tag in project.tags"
                  :key="tag"
                  class="text-xs bg-gray-100 text-gray-700 px-2 py-1 rounded-full"
                >
                    {{ tag }}
                </span>
            </div>

            <div class="flex gap-4 mt-4 text-sm font-medium">
                <a :href="project.liveUrl" class="text-blue-600 hover:underline">Live Demo</a>
                <a :href="project.repoUrl" class="text-blue-600 hover:underline">Repository</a>
            </div>
        </div>
    </div>
</template>