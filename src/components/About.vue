<template>
  <section id="about" class="py-20 md:py-32">
    <div class="grid md:grid-cols-2 gap-12 items-center">
      <div>
        <h2 class="text-4xl md:text-5xl font-bold text-white mb-6">
          Sobre Mim
        </h2>
        <p class="text-slate-300 text-lg leading-relaxed mb-4">
          Sou Gil Anderson, desenvolvedor Full Stack com experiência em
          aplicações web e mobile, especializado em Vue.js, Angular, Ionic,
          Laravel e Nest.js. Tenho atuado em projetos que vão desde o
          desenvolvimento de interfaces modernas e responsivas até a criação de
          APIs escaláveis e seguras, sempre com foco em performance, organização
          e qualidade de código.
        </p>
        <p class="text-slate-300 text-lg leading-relaxed mb-6">
          Sou apaixonado por tecnologia e pela criação de soluções que unam
          funcionalidade e experiência do usuário. Valorizo boas práticas,
          clareza e manutenibilidade no desenvolvimento, buscando constantemente
          aprimorar minhas habilidades e entregar resultados que façam a
          diferença para pessoas e negócios.
        </p>
        <div class="flex gap-4">
          <a
            href="https://github.com/gil-gomes"
            class="text-cyan-400 hover:text-cyan-300 transition-colors"
            target="_blank"
            >GitHub
          </a>
          <a
            href="https://www.linkedin.com/in/gil-anderson-gomes-67696a125/"
            class="text-cyan-400 hover:text-cyan-300 transition-colors"
            target="_blank"
            >LinkedIn
          </a>
        </div>
      </div>
      <div
        class="bg-linear-to-br from-cyan-400/20 to-blue-500/20 rounded-lg p-8 border border-cyan-400/30"
      >
        <div class="space-y-4">
          <div class="flex items-center gap-3">
            <span class="text-2xl">🎓</span>
            <div>
              <h3 class="text-white font-semibold">Educação</h3>
              <p class="text-slate-400 text-sm">
                Licenciatura em Computação – Instituto Federal do Sertão
                Pernambucano (IF Sertão-PE) – Campus Petrolina
              </p>
              <p class="text-slate-400 text-sm">
                Ensino Médio Técnico em Informática – CETEP Sertão do São
                Francisco
              </p>
            </div>
          </div>
          <div class="flex items-center gap-3">
            <span class="text-2xl">💼</span>
            <div>
              <h3 class="text-white font-semibold">Experiência</h3>
              <p class="text-slate-400 text-sm">+3 anos em desenvolvimento</p>
            </div>
          </div>
          <div class="flex items-center gap-3">
            <span class="text-2xl">🚀</span>
            <div>
              <h3 class="text-white font-semibold">Projetos</h3>
              <p class="text-slate-400 text-sm">15+ projetos concluídos</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts"></script>
