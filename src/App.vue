<template>
  <div class="min-h-screen bg-neutral-900 text-slate-100">
    <Navigation />
    <main class="max-w-7xl m-auto px-4 sm:px-6 lg:px-8">
      <Hero />
      <About />
      <Skills />
      <Experience />
      <Projects />
      <Contact />
    </main>
    <Footer />
  </div>
</template>

<script setup lang="ts">
import Navigation from "./components/Navigation.vue";
import Hero from "./components/Hero.vue";
import About from "./components/About.vue";
import Skills from "./components/Skills.vue";
import Experience from "./components/Experience.vue";
import Projects from "./components/Projects.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";
</script>

<style>
html {
  scroll-behavior: smooth;
}
</style>
