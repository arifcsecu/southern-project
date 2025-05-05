<template>
  <header class="bg-gray-800 text-white py-4">
    <div class="container mx-auto flex justify-between items-center px-4">
      <h1 class="text-xl font-bold">My Nuxt Site</h1>
      <nav class="space-x-4">
        <NuxtLink to="/" class="hover:underline">Home</NuxtLink>
        <NuxtLink to="/about" class="hover:underline">About</NuxtLink>
      </nav>
    </div>
  </header>
</template>
