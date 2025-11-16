<template>
  <section id="projects" class="py-20 md:py-32">
    <h2 class="text-4xl md:text-5xl font-bold text-white mb-12 text-center">
      Projetos Destacados
    </h2>

    <div class="grid md:grid-cols-2 gap-8">
      <div
        v-for="project in projects"
        :key="project.id"
        class="group bg-slate-800/50 border border-slate-700 rounded-lg overflow-hidden hover:border-cyan-400/50 transition-all"
      >
        <div
          class="h-48 bg-linear-to-br from-cyan-400/20 to-blue-500/20 flex items-center justify-center"
        >
          <span class="text-6xl">{{ project.icon }}</span>
        </div>
        <div class="p-8">
          <h3 class="text-2xl font-bold text-white mb-2">{{ project.name }}</h3>
          <p class="text-slate-300 mb-4">{{ project.description }}</p>
          <div class="flex flex-wrap gap-2 mb-6">
            <span
              v-for="tech in project.technologies"
              :key="tech"
              class="px-3 py-1 bg-cyan-400/10 text-cyan-400 rounded-full text-sm"
            >
              {{ tech }}
            </span>
          </div>
          <div class="flex gap-4">
            <a
              :href="project.liveUrl || '#'"
              target="_blank"
              rel="noopener noreferrer"
              class="text-cyan-400 hover:text-cyan-300 transition-colors font-semibold"
              >Ver Projeto →</a
            >
            <a
              :href="project.githubUrl || '#'"
              target="_blank"
              rel="noopener noreferrer"
              class="text-slate-400 hover:text-slate-300 transition-colors"
              >GitHub
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
type Project = {
  id: number;
  name: string;
  description: string;
  icon: string;
  technologies: string[];
  liveUrl?: string;
  githubUrl?: string;
};

const projects: Project[] = [
  {
    id: 1,
    name: "Conversor de Moedas Online",
    description:
      "Aplicação web para converter valores entre moedas em tempo real usando a API pública exchangerate.host. Interface direta com feedback visual, transparência na fonte das taxas, tratamento de erros e responsividade para dispositivos móveis.",
    icon: "🪙",
    technologies: [
      "HTML",
      "CSS",
      "JavaScript",
      "exchangerate.host API",
      "Netlify",
    ],
    liveUrl: "https://conversionmoney.netlify.app/",
    githubUrl: "https://github.com/gil-gomes/conversor-de-moedas",
  },
  {
    id: 2,
    name: "Site de Casamento — Emilly & Gil",
    description:
      "Website de casamento com design elegante, interatividade e integração em tempo real. Convidados acessam informações do evento, lista de presentes e contagem regressiva. Desenvolvido com Vue.js e Tailwind CSS, responsivo e com dados sincronizados via Firebase.",
    icon: "💍",
    technologies: ["Vue.js", "Tailwind CSS", "Firebase (Firestore)", "Netlify"],
    liveUrl: "https://emilly-gil-anderson.netlify.app/#/",
    githubUrl: "https://github.com/gil-gomes/site-casamento",
  },
];
</script>
