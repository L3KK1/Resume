<!-- src/components/Navbar.vue -->
<template>
  <nav class="fixed top-0 w-full bg-zinc-950/95 backdrop-blur-lg border-b border-zinc-800 z-50">
    <div class="max-w-6xl mx-auto px-5 py-5 flex justify-between items-center">
      <div class="text-2xl font-bold">В. Лещинский</div>

      <!-- Десктоп меню -->
      <div class="hidden md:flex items-center gap-8 text-sm">
        <a href="#about" class="hover:text-cyan-400 transition">Обо мне</a>
        <a href="#projects" class="hover:text-cyan-400 transition">Проекты</a>
        <a href="#skills" class="hover:text-cyan-400 transition">Навыки</a>
        <a href="#education" class="hover:text-cyan-400 transition">Образование</a>
        <a href="#contact" class="hover:text-cyan-400 transition">Контакты</a>
      </div>

      <!-- Мобильная кнопка -->
      <button @click="isMenuOpen = !isMenuOpen" class="md:hidden text-2xl">
        {{ isMenuOpen ? '✕' : '☰' }}
      </button>
    </div>

    <!-- Мобильное меню -->
    <div v-if="isMenuOpen" class="md:hidden bg-zinc-900 border-t border-zinc-800">
      <div class="flex flex-col py-4 text-center text-lg">
        <a href="#about" @click="isMenuOpen = false" class="py-4 hover:bg-zinc-800">Обо мне</a>
        <a href="#projects" @click="isMenuOpen = false" class="py-4 hover:bg-zinc-800">Проекты</a>
        <a href="#skills" @click="isMenuOpen = false" class="py-4 hover:bg-zinc-800">Навыки</a>
        <a href="#education" @click="isMenuOpen = false" class="py-4 hover:bg-zinc-800">Образование</a>
        <a href="#contact" @click="isMenuOpen = false" class="py-4 hover:bg-zinc-800">Контакты</a>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue'
const isMenuOpen = ref(false)
</script>