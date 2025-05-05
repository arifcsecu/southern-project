<template>
    <section class="container mx-auto px-4 mb-6 mt-4">
        <!-- Title + See All -->
        <div class="flex justify-between items-center mb-1 px-2 md:px-0">
            <h2 class="text-lg md:text-xl font-bold">একাডেমিক ইনফরমেশন</h2>
            <a href="#" class="text-xs md:text-sm text-red-500 hover:underline">See All</a>
        </div>

        <!-- Red Bottom Line -->
        <div class="w-6 h-1 bg-red-400 mb-3"></div>

        <!-- Horizontal Scroll Tabs -->
        <div class="flex items-center space-x-2 overflow-x-auto no-scrollbar px-2 md:px-0">
            <!-- Left Scroll Arrow -->
            <button class="w-8 h-8 flex items-center justify-center rounded-full bg-gray-100">
                <span>&lt;</span>
            </button>

            <button
                v-for="(tab, index) in tabs"
                :key="index"
                class="px-4 py-2 rounded-full text-xs md:text-sm whitespace-nowrap"
                :class="index === 0 ? 'bg-red-400 text-white' : 'bg-gray-100 text-gray-800'"
            >
                {{ tab }}
            </button>

            <button class="w-8 h-8 flex items-center justify-center rounded-full bg-gray-100">
                <span>&gt;</span>
            </button>
        </div>
    </section>
</template>

<script setup>
const tabs = [
    'School',
    'College',
    'University',
    'Curriculum & Syllabus',
    'Exam Routine',
    'Result',
    'Public University',
    'Private University',
]
</script>

<style scoped>
.no-scrollbar::-webkit-scrollbar {
    display: none;
}
.no-scrollbar {
    -ms-overflow-style: none;
    scrollbar-width: none;
}

@media (max-width: 768px) {
    h2 {
        font-size: 1rem; /* Adjust title size for smaller screens */
    }
    a {
        font-size: 0.875rem; /* Adjust link size for smaller screens */
    }
    button {
        font-size: 0.75rem; /* Adjust button text size for smaller screens */
    }
}
</style>