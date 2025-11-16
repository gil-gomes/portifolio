<template>
  <nav
    class="sticky top-0 z-50 bg-slate-900/95 backdrop-blur-sm border-b border-slate-700"
  >
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <div class="flex-shrink-0">
          <a
            href="#"
            class="text-2xl font-bold bg-linear-to-r from-cyan-400 to-blue-500 bg-clip-text text-transparent"
          >
            Gil Gomes
          </a>
        </div>
        <div class="hidden md:flex space-x-8">
          <a
            href="#about"
            class="text-slate-300 hover:text-cyan-400 transition-colors"
            >Sobre</a
          >
          <a
            href="#skills"
            class="text-slate-300 hover:text-cyan-400 transition-colors"
            >Habilidades</a
          >
          <a
            href="#experience"
            class="text-slate-300 hover:text-cyan-400 transition-colors"
            >Experiência</a
          >
          <a
            href="#projects"
            class="text-slate-300 hover:text-cyan-400 transition-colors"
            >Projetos</a
          >
          <a
            href="#contact"
            class="text-slate-300 hover:text-cyan-400 transition-colors"
            >Contato</a
          >
        </div>
        <button class="md:hidden text-slate-300 hover:text-cyan-400">
          <svg
            class="w-6 h-6"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16"
            />
          </svg>
        </button>
      </div>
    </div>
  </nav>
</template>

<script setup lang="ts"></script>
