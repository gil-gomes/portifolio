<template>
  <section id="skills" class="py-16 md:py-24">
    <h2 class="text-4xl md:text-5xl font-bold text-white mb-12 text-center">
      Habilidades Técnicas
    </h2>

    <div class="grid md:grid-cols-3 gap-8">
      <div
        v-for="category in skillCategories"
        :key="category.name"
        class="bg-slate-800/50 border border-slate-700 rounded-lg p-8 hover:border-cyan-400/50 transition-all"
      >
        <h3 class="text-2xl font-bold text-cyan-400 mb-6">
          {{ category.name }}
        </h3>
        <div class="space-y-3">
          <div
            v-for="skill in category.skills"
            :key="skill"
            class="flex items-center gap-2"
          >
            <span class="w-2 h-2 bg-cyan-400 rounded-full"></span>
            <span class="text-slate-300">{{ skill }}</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
const skillCategories = [
  {
    name: "Front-end",
    skills: [
      "HTML",
      "CSS",
      "JavaScript",
      "TypeScript",
      "Vue.js",
      "Angular",
      "Ionic",
      "Quasar",
      "Bootstrap",
      "Tailwind CSS",
      "Chakra UI",
    ],
  },
  {
    name: "Back-end",
    skills: ["Node.js", "PHP", "Laravel", "Nest.js", "MySQL"],
  },
  {
    name: "Ferramentas e Controle de Versão",
    skills: ["Git", "GitHub", "GitLab", "Trello",],
  },
];
</script>
