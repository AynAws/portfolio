<script setup>
defineProps({
    full: { type: String, required: true },
    link: { type: String, default: null }
})
</script>

<template>
    <span class="relative group cursor-help border-b border-dotted border-current">
        <slot />
        <span
          class="pointer-events-none absolute left-1/2 -translate-x-1/2 bottom-full mb-0 w-56 opacity-0 scale-95 group-hover:opacity-100 group-hover:scale-100 group-hover:pointer-events-auto transition-all duration-200 bg-indigo-custom text-white text-xs rounded-md p-2 z-10 shadow-lg"
        >
            {{ full }}
            <a v-if="link" :href="link" target="_blank" rel="noopener" class="block mt-1 underline">
                Visit site →
            </a>
        </span>
    </span>
</template>