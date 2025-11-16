<template>
  <section id="experience" class="py-20 md:py-32">
    <h2 class="text-4xl md:text-5xl font-bold text-white mb-12 text-center">Experiência Profissional</h2>
    
    <div class="space-y-8">
      <div v-for="(job, index) in experiences" :key="index" class="bg-slate-800/50 border border-slate-700 rounded-lg p-8 hover:border-cyan-400/50 transition-all">
        <div class="flex flex-col md:flex-row md:items-center md:justify-between mb-4">
          <div>
            <h3 class="text-2xl font-bold text-white">{{ job.position }}</h3>
            <p class="text-cyan-400">{{ job.company }}</p>
          </div>
          <span class="text-slate-400 text-sm mt-2 md:mt-0">{{ job.period }}</span>
        </div>
        <p class="text-slate-300 leading-relaxed">{{ job.description }}</p>
        <div class="flex flex-wrap gap-2 mt-4">
          <span v-for="tech in job.technologies" :key="tech" class="px-3 py-1 bg-cyan-400/10 text-cyan-400 rounded-full text-sm">
            {{ tech }}
          </span>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
const experiences = [
  {
    position: 'Desenvolvedor Front-end Freelancer — Projeto Web Vue 3',
    company: 'Freelancer',
    period: 'Mar/2024 – Abr/2025',
    description: 'Desenvolvimento de aplicação web com Vue.js 3, focando em performance, escalabilidade e qualidade de código. Criação de componentes reutilizáveis, integração com APIs RESTful e gerenciamento de estado com Pinia.',
    technologies: ['Vue 3', 'TypeScript', 'Pinia', 'Axios', 'Tailwind']
  },
  {
    position: 'Desenvolvedor Front-end Freelancer — Editor de Imagens e Vídeos',
    company: 'Freelancer',
    period: 'Abr/2024 – Jan/2025',
    description: 'Desenvolvimento de aplicação avançada para edição de imagens e vídeos em Angular, com renderização em Canvas e uso de Web Workers para otimização de performance.',
    technologies: ['Angular', 'RxJS', 'TypeScript', 'Canvas', 'Web Workers']
  },
  {
    position: 'Desenvolvedor Front-end Freelancer',
    company: 'Freelancer',
    period: 'Jan/2023 – Mar/2024',
    description: 'Criação de interfaces modernas e responsivas com Vue.js e Quasar, utilizando Pinia para gerenciamento de estado e integração com APIs RESTful.',
    technologies: ['Vue.js', 'Quasar', 'Pinia', 'Axios']
  },
  {
    position: 'Desenvolvedor Full Stack Freelancer — Calculadora de Alimentos',
    company: 'Freelancer',
    period: 'Ago/2023 – Fev/2024',
    description: 'Desenvolvimento completo de uma ferramenta nutricional, desde o design da interface até a integração com APIs externas. Foco em reuso de componentes e usabilidade.',
    technologies: ['Vue.js', 'Laravel', 'Pinia', 'REST API']
  },
  {
    position: 'Desenvolvedor Full Stack Freelancer — Instituto Coelho',
    company: 'Freelancer',
    period: 'Nov/2021 – Mar/2022',
    description: 'Criação de sistema para cadastro de usuários, consultas e contratos, com integração de APIs REST e autenticação segura.',
    technologies: ['Laravel', 'Vue.js', 'REST API', 'MySQL']
  },
  {
    position: 'Desenvolvedor Back-end — Pactus',
    company: 'Pactus',
    period: 'Jul/2021 – Dez/2022',
    description: 'Arquitetura e desenvolvimento de APIs REST escaláveis, otimização de consultas SQL e colaboração direta com o time front-end para integração eficiente.',
    technologies: ['Node.js', 'Nest.js', 'MySQL', 'REST API']
  },
  {
    position: 'Desenvolvedor Full Stack — Atena Agência',
    company: 'Atena Agência',
    period: 'Dez/2020 – Out/2021',
    description: 'Desenvolvimento de aplicativo para contratação de serviços, com autenticação via Laravel Sanctum e integração de múltiplas APIs.',
    technologies: ['Laravel', 'Vue.js', 'Sanctum', 'MySQL']
  }
]
</script>
