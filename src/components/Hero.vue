<template>
  <section class="py-20 md:py-32 flex items-center justify-center">
    <div class="text-center">
      <div class="mb-8">
        <div
          class="w-24 h-24 mx-auto rounded-full bg-linear-to-br from-cyan-400 to-blue-500 p-1"
        >
          <div
            class="w-full h-full rounded-full bg-slate-900 flex items-center justify-center"
          >
            <span class="text-4xl">👨‍💻</span>
          </div>
        </div>
      </div>
      <h1 class="text-5xl md:text-7xl font-bold text-white mb-6 text-balance">
        Desenvolvedor Full Stack
      </h1>
      <p
        class="text-xl md:text-2xl text-slate-300 mb-8 max-w-2xl mx-auto text-balance"
      >
        Especializado em <span class="text-cyan-400 font-semibold">Vue 3</span>,
        <span class="text-cyan-400 font-semibold">Angular</span> e
        <span class="text-cyan-400 font-semibold">Node.js</span>
      </p>
      <div class="flex flex-col sm:flex-row gap-4 justify-center">
        <a
          href="#projects"
          class="px-8 py-3 bg-linear-to-r from-cyan-400 to-blue-500 text-slate-900 font-semibold rounded-lg hover:shadow-lg hover:shadow-cyan-400/50 transition-all"
        >
          Ver Projetos
        </a>
        <a
          href="#contact"
          class="px-8 py-3 border-2 border-cyan-400 text-cyan-400 font-semibold rounded-lg hover:bg-cyan-400/10 transition-all"
        >
          Entrar em Contato
        </a>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts"></script>
