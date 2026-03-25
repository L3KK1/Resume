<template>
  <div class="min-h-screen bg-zinc-950 text-zinc-200">
    <Navbar />
    
    <main>
      <Hero />
      <About />
      <Projects />
      <Skills />
      <Education />
      <Contact />
    </main>

    <Footer />
  </div>
</template>

<script setup>
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Projects from './components/Projects.vue'
import Skills from './components/Skills.vue'
import Education from './components/Education.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'
</script>