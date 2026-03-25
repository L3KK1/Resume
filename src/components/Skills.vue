<template>
  <section id="skills" class="py-24 bg-zinc-900">
    <div class="max-w-6xl mx-auto px-6">
      <h2 class="text-4xl font-bold text-center mb-16">Навыки</h2>

      <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
        <div v-for="skill in skills" :key="skill" 
             class="bg-zinc-800 hover:bg-zinc-700 transition p-6 rounded-3xl text-center">
          <div class="text-4xl mb-4">{{ getIcon(skill) }}</div>
          <p class="font-medium">{{ skill }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const skills = [
  "C++", "SQL", "Embedded C", "JavaScript", 
  "Kotlin", "MS SQL Server", "Node.js", "Vue.js",
  "Android Studio", "Git", "Linux", "Информационная безопасность"
]

const getIcon = (skill) => {
  const icons = {
    "C++": "💻",
    "SQL": "🗄️",
    "Embedded C": "🔌",
    "JavaScript": "🟨",
    "Kotlin": "📱",
    "MS SQL Server": "🗃️",
    "Node.js": "⚡",
    "Vue.js": "🌊",
    "Android Studio": "🤖",
    "Git": "🐙",
    "Linux": "🐧",
    "Информационная безопасность": "🛡️"
  }
  return icons[skill] || "🔧"
}
</script>