<template>
  <section id="comparatif" class="relative py-32 bg-[#050B19] overflow-hidden">

    <!-- Background Grid -->
    <div class="absolute inset-0 grid-bg opacity-[0.07]"></div>

    <div class="relative z-10 max-w-7xl mx-auto px-6 md:px-12 lg:px-20">

      <h2 class="text-center text-4xl md:text-5xl font-bold text-white mb-20 neon-title">
        Sans Agent IA vs Avec Agent IA
      </h2>

      <div class="grid lg:grid-cols-2 gap-16">

        <!-- Sans Agent IA -->
        <div class="comp-card reveal">
          <h3 class="comp-title text-red-400">❌ Sans Agent IA</h3>
          <ul class="comp-list space-y-4">
            <li>⛔ Tâches manuelles répétitives</li>
            <li>⛔ Perte de temps à chercher l'information</li>
            <li>⛔ Support client lent et coûteux</li>
            <li>⛔ Erreurs humaines fréquentes</li>
            <li>⛔ Faible exploitation du savoir interne</li>
          </ul>
        </div>

        <!-- Avec Agent IA -->
        <div class="comp-card reveal">
          <h3 class="comp-title text-[#2EC4B6]">✔ Avec Agent IA + RAG</h3>
          <ul class="comp-list space-y-4">
            <li>✅ Automatisation avancée</li>
            <li>✅ Réponses fiables basées sur vos documents</li>
            <li>✅ Support client instantané 24/7</li>
            <li>✅ Réduction des erreurs humaines</li>
            <li>✅ Productivité boostée au sein de l’équipe</li>
          </ul>
        </div>

      </div>

    </div>
  </section>
</template>

<script setup>
import { onMounted } from 'vue'
import ScrollReveal from 'scrollreveal'

onMounted(() => {
  ScrollReveal().reveal('.reveal', {
    duration: 1200,
    distance: '40px',
    origin: 'bottom',
    interval: 200,
    easing: 'ease-in-out'
  })
})
</script>

<style scoped>
/* Grid */
.grid-bg {
  background: linear-gradient(#2ec4b615 1px, transparent 1px),
              linear-gradient(90deg, #2ec4b615 1px, transparent 1px);
  background-size: 55px 55px;
  animation: gridMove 18s linear infinite;
}
@keyframes gridMove {
  0% { background-position: 0 0, 0 0; }
  100% { background-position: 120px 120px, 120px 120px; }
}

/* Title */
.neon-title {
  text-shadow: 0 0 10px #2EC4B6, 0 0 25px #2EC4B6;
}

/* Card */
.comp-card {
  background: rgba(255, 255, 255, 0.03);
  border: 1px solid rgba(255, 255, 255, 0.07);
  padding: 2.5rem;
  border-radius: 1.5rem;
  backdrop-filter: blur(14px);
  box-shadow: 0 0 20px rgba(46, 196, 182, 0.09);
  transition: all 0.4s ease;
}
.comp-card:hover {
  transform: translateY(-10px) scale(1.02);
  border-color: rgba(46, 196, 182, 0.7);
  box-shadow: 0 0 28px rgba(46, 196, 182, 0.3), 0 0 40px rgba(106, 60, 255, 0.25);
}

/* Titles */
.comp-title {
  font-size: 1.8rem;
  font-weight: 600;
  margin-bottom: 1.4rem;
  text-shadow: 0 0 10px rgba(255, 255, 255, 0.2);
}

/* List */
.comp-list li {
  font-size: 1.05rem;
  color: #d0e0f0;
  line-height: 1.7;
}
</style>
