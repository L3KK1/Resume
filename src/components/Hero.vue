<!-- src/components/Hero.vue -->
<template>
  <section class="min-h-screen flex items-center pt-20 pb-16">
    <div class="max-w-6xl mx-auto px-6 grid md:grid-cols-2 gap-12 items-center">
      <div class="text-center md:text-left">
        <h1 class="text-5xl md:text-7xl font-bold leading-tight mb-6">
          Владимир Лещинский
        </h1>
        <p class="text-2xl md:text-3xl text-cyan-400 mb-6">
          Специалист по информационной безопасности
        </p>
        <p class="text-lg md:text-xl text-zinc-400 max-w-lg mx-auto md:mx-0">
          Студент БГУ. Опыт в разработке баз данных, веб-приложений и мобильных решений.
        </p>

        <div class="flex flex-col sm:flex-row gap-4 mt-10 justify-center md:justify-start">
          <a href="#contact" 
             class="px-8 py-4 bg-cyan-500 hover:bg-cyan-600 text-zinc-950 font-semibold rounded-2xl text-center transition">
            Связаться со мной
          </a>
          <a href="#projects" 
             class="px-8 py-4 border border-zinc-600 hover:border-cyan-400 rounded-2xl text-center transition">
            Мои проекты
          </a>
        </div>
      </div>

      <div class="flex justify-center mt-10 md:mt-0">
        <div class="w-64 h-64 md:w-80 md:h-80 bg-gradient-to-br from-cyan-400 to-blue-600 rounded-full p-2">
          <div class="w-full h-full bg-zinc-950 rounded-full flex items-center justify-center text-9xl">
            🛡️
          </div>
        </div>
      </div>
    </div>
  </section>
</template>