<!-- src/components/Projects.vue -->
<template>
  <section id="projects" class="py-20 md:py-24 bg-zinc-900">
    <div class="max-w-6xl mx-auto px-6">
      <h2 class="text-4xl font-bold text-center mb-12">Проекты</h2>

      <div class="grid md:grid-cols-2 gap-8">
        <div v-for="(project, i) in projects" :key="i"
             class="bg-zinc-800 rounded-3xl overflow-hidden hover:scale-[1.02] transition-all">
          <div class="h-52 bg-zinc-700 flex items-center justify-center text-7xl">
            {{ project.emoji }}
          </div>
          <div class="p-7">
            <div class="flex justify-between mb-4">
              <h3 class="text-xl font-semibold">{{ project.title }}</h3>
              <span class="text-xs bg-zinc-700 px-3 py-1 rounded-full">{{ project.year }}</span>
            </div>
            <p class="text-zinc-400 text-sm leading-relaxed mb-6">{{ project.desc }}</p>
            <div class="flex flex-wrap gap-2">
              <span v-for="tech in project.tech" :key="tech"
                    class="text-xs bg-zinc-900 px-4 py-1.5 rounded-full text-cyan-300">
                {{ tech }}
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const projects = [
  {
    title: "Веб-приложение библиотеки",
    desc: "Полноценное приложение с подключением MS SQL Server через Node.js и Vue.js интерфейсом.",
    emoji: "📚",
    year: "2026",
    tech: ["Vue.js", "Node.js", "MS SQL"]
  },
  {
    title: "Реляционная база данных",
    desc: "Проектирование и реализация БД на MS SQL с CRUD-операциями и ограничениями целостности.",
    emoji: "🗄️",
    year: "2026",
    tech: ["MS SQL Server", "SQL"]
  },
  {
    title: "Мобильное приложение на Kotlin",
    desc: "Android-приложение с современным UI и интеграцией внешних API.",
    emoji: "📱",
    year: "2023",
    tech: ["Kotlin", "Android Studio"]
  }
]
</script>