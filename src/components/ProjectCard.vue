<script setup>
defineProps(['project'])
</script>

<template>
    <div class="group rounded-xl bg-white shadow-md overflow-hidden flex flex-col transition-all duration-300 hover:-translate-y-2 hover:shadow-xl">
        <div class="shimmer">
            <img :src="project.image" :alt="project.alt" class="w-full h-40 object-cover">
        </div>

        <div class="p-5 flex flex-col flex-1 text-indigo-custom">
            <h3 class="text-lg font-bold">{{ project.title }}</h3>
            <p class="text-sm mt-2 flex-1 text-gray-600">{{ project.desc }}</p>

            <div class="flex flex-wrap mt-4">
                <span
                  v-for="tag in project.tags"
                  :key="tag"
                  class="text-xs bg-cream px-2 py-1 rounded-full font-medium"
                >
                    {{ tag }}
                </span>
            </div>

            <div class="flex gap-4 mt-4 text-sm font-medium underline-grow [&>a]:text-indigo-custom">
                <a :href="project.liveUrl">Live Demo</a>
                <a :href="project.repoUrl">Repository</a>
            </div>
        </div>
    </div>
</template>