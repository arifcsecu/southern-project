<template>
  <div class="min-h-screen flex flex-col">
    <Header1 />
    <Header2 />
    <Header3 />
    <Navbar />
    <main class="container mx-auto py-6 flex-grow">
      <NuxtPage />
    </main>
    <Footer />
  </div>
</template>

<script setup>
import Header3 from "~/components/Header3.vue";
import Header2 from "~/components/Header2.vue";
import Header1 from "~/components/Header1.vue";
import Navbar from "~/components/Navbar.vue";
import Footer from "~/components/Footer.vue";
</script>
