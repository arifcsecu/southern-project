<template>
  <div>
    <Navbar />
    <main class="container mx-auto py-6">
      <NuxtPage />
    </main>
    <Footer />
  </div>
</template>

<script setup>
import Navbar from "~/components/Navbar.vue";
import Footer from "~/components/Footer.vue";
</script>
