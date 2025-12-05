<template>
  <section id="rag" class="relative py-32 bg-[#050B19] overflow-hidden">

    <!-- Animated Grid Background -->
    <div class="absolute inset-0 grid-bg opacity-[0.07]"></div>

    <div class="relative z-10 max-w-7xl mx-auto px-6 md:px-12 lg:px-20">
      <h2 class="text-center text-4xl md:text-5xl font-bold text-white mb-20 neon-title">
        Qu’est‑ce que le RAG ?
      </h2>

      <div class="grid lg:grid-cols-2 gap-16">

        <!-- Card: Simple Definition -->
        <div class="rag-card reveal">
          <h3 class="rag-title">Définition simple</h3>
          <p class="rag-text">
            Le RAG (Retrieval‑Augmented Generation) est une technologie qui permet à votre
            intelligence artificielle de <span class="highlight">chercher automatiquement les bonnes informations</span>
            dans vos documents internes (PDF, emails, fiches produits, rapports…) AVANT de répondre.
          </p>
          <p class="rag-text mt-4">
            Résultat : l’IA fournit des réponses <span class="highlight">fiables, vérifiées et spécifiques</span> à votre
            entreprise, et non des réponses génériques prises sur Internet.
          </p>
        </div>

        <!-- Card: Why it's essential -->
        <div class="rag-card reveal">
          <h3 class="rag-title">Pourquoi c’est indispensable</h3>
          <ul class="rag-list space-y-4">
            <li>✔ Réponses basées sur VOS documents internes</li>
            <li>✔ Réduction immédiate des erreurs humaines</li>
            <li>✔ Vos équipes gagnent un temps précieux</li>
            <li>✔ Vous exploitez enfin tout votre savoir interne</li>
            <li>✔ Idéal pour le support client, l’analyse, la formation</li>
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
/* Animated Grid */
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

/* Neon Title */
.neon-title {
  text-shadow: 0 0 10px #2EC4B6, 0 0 25px #2EC4B6;
}

/* RAG Cards */
.rag-card {
  background: rgba(255, 255, 255, 0.03);
  border: 1px solid rgba(255, 255, 255, 0.07);
  padding: 2.5rem;
  border-radius: 1.5rem;
  backdrop-filter: blur(14px);
  box-shadow: 0 0 20px rgba(46, 196, 182, 0.09);
  transition: all 0.4s ease;
}
.rag-card:hover {
  transform: translateY(-10px) scale(1.02);
  border-color: rgba(46, 196, 182, 0.7);
  box-shadow: 0 0 28px rgba(46, 196, 182, 0.3), 0 0 40px rgba(106, 60, 255, 0.25);
}

/* Titles */
.rag-title {
  font-size: 1.8rem;
  font-weight: 600;
  color: white;
  margin-bottom: 1rem;
  text-shadow: 0 0 10px rgba(46,196,182,0.5);
}

/* Text */
.rag-text {
  color: #b9c7d7;
  line-height: 1.7;
  font-size: 1.05rem;
}
.highlight {
  color: #2EC4B6;
  font-weight: 600;
}

/* List */
.rag-list li {
  color: #d0e0f0;
  font-size: 1.05rem;
  padding-left: 8px;
}
.rag-list li::marker {
  color: #2EC4B6;
  font-weight: bold;
}
</style>
