<!-- src/components/Contact.vue -->
<template>
  <section id="contact" class="py-24 bg-zinc-900">
    <div class="max-w-4xl mx-auto px-6 text-center">
      <h2 class="text-4xl font-bold mb-8">Связаться со мной</h2>
      <p class="text-zinc-400 text-lg mb-12 max-w-md mx-auto">
        Открыт к предложениям стажировок, проектам и сотрудничеству в сфере информационной безопасности
      </p>

      <div class="flex flex-col sm:flex-row gap-4 justify-center mb-12">
        <a href="mailto:lebe6kun@gmail.com" 
           class="flex items-center justify-center gap-3 bg-zinc-800 hover:bg-zinc-700 transition px-8 py-4 rounded-2xl text-lg">
          <span class="text-2xl">✉️</span>
          <span>lebe6kun@gmail.com</span>
        </a>

        <a href="tel:+375291684934" 
           class="flex items-center justify-center gap-3 bg-zinc-800 hover:bg-zinc-700 transition px-8 py-4 rounded-2xl text-lg">
          <span class="text-2xl">📱</span>
          <span>+375 (29) 168-49-34</span>
        </a>
      </div>

      <!-- Социальные сети -->
      <div class="flex justify-center gap-8 text-4xl">
        <!-- Telegram -->
       <a href="https://t.me/nelebe6" target="_blank"
   class="text-[#229ED9] hover:scale-110 transition-transform">
  <svg xmlns="http://www.w3.org/2000/svg" width="48" height="48" fill="currentColor" viewBox="0 0 24 24">
    <path d="M9.417 15.181l-.397 5.584c.568 0 .814-.244 1.109-.537l2.663-2.545 5.518 4.041c1.012.564 1.725.267 1.998-.931L21 4.308c.27-1.285-.923-1.86-2.01-1.32L3.5 9.5c-1.285.486-1.28 1.285-.18 1.61l4.11 1.28 9.55-5.99c.46-.29.88.18.44.48L9.417 15.181z"/>
  </svg>
</a>
        <!--GitHub --> 
        <a href="https://github.com/L3KK1" target="_blank" class="hover:text-white transition">
          <svg xmlns="http://www.w3.org/2000/svg" width="44" height="44" viewBox="0 0 24 24" fill="currentColor">
            <path d="M12 0C5.374 0 0 5.373 0 12c0 5.302 3.438 9.8 8.207 11.387.6.113.793-.26.793-.577 0-.285-.01-1.044-.015-2.05-3.338.726-4.042-1.416-4.042-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.744.083-.729.083-.729 1.205.084 1.84 1.237 1.84 1.237 1.07 1.834 2.807 1.304 3.492.997.108-.775.418-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.4 3-.405 1.02.005 2.04.138 3 .405 2.29-1.552 3.29-1.23 3.29-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.604-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 21.795 24 17.3 24 12c0-6.627-5.373-12-12-12z"/>
          </svg>
        </a>

      </div>
    </div>
  </section>
</template>