<script setup>
import Navbar from "./components/Navbar.vue";
import Hero from "./components/Hero.vue";
import Features from "./components/Features.vue";
import Statistics from "./components/Statistics.vue";
import Screenshots from "./components/Screenshots.vue";
import FAQ from "./components/FAQ.vue";
import Download from "./components/Download.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <div class="bg-[#09080E] text-white overflow-x-hidden">
    <Navbar />
    <Hero />
    <Features />
    <Statistics />
    <Screenshots />
    <Download />
    <FAQ />
    <Footer />
  </div>
</template>