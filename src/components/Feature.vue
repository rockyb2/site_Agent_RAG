<template>
  <section id="features" class="relative py-32 bg-[#050B19] overflow-hidden">

    <!-- Background Grid -->
    <div class="absolute inset-0 grid-bg opacity-[0.1]"></div>

    <div class="relative z-10 max-w-7xl mx-auto px-6 md:px-12 lg:px-20">
      <h2 class="text-center text-4xl md:text-5xl font-bold text-white mb-20 neon-title">
        Les besoins actuels des entreprises
      </h2>

      <div class="grid md:grid-cols-3 gap-12">

        <!-- Card 1 -->
        <div class="feature-card group">
          <div class="icon-circle">
            <i class="fa-solid fa-robot"></i>
          </div>
          <h3 class="feature-title">Automatisation</h3>
          <p class="feature-text">
            Trop de tâches répétitives gaspillent du temps que vos équipes pourraient consacrer à des activités à forte valeur.
          </p>
        </div>

        <!-- Card 2 -->
        <div class="feature-card group">
          <div class="icon-circle">
            <i class="fa-solid fa-headset"></i>
          </div>
          <h3 class="feature-title">Support Client</h3>
          <p class="feature-text">
            Les entreprises cherchent à réduire les coûts du support client tout en offrant des réponses rapides et cohérentes.
          </p>
        </div>

        <!-- Card 3 -->
        <div class="feature-card group">
          <div class="icon-circle">
            <i class="fa-solid fa-database"></i>
          </div>
          <h3 class="feature-title">Gestion de l'information</h3>
          <p class="feature-text">
            Vos données internes sont précieuses, mais souvent difficilement exploitables sans outils intelligents.
          </p>
        </div>

      </div>
    </div>

  </section>
</template>

<script setup>
import { onMounted } from 'vue'
import ScrollReveal from 'scrollreveal'

onMounted(() => {
  ScrollReveal().reveal('.feature-card', {
    duration: 1200,
    distance: '40px',
    origin: 'bottom',
    interval: 200,
    easing: 'ease-in-out'
  })
})
</script>

<style scoped>
/* GRID BACKGROUND */
.grid-bg {
  background: linear-gradient(#2ec4b615 1px, transparent 1px),
              linear-gradient(90deg, #2ec4b615 1px, transparent 1px);
  background-size: 50px 50px;
  animation: moveGrid 15s linear infinite;
}
@Override
@keyframes moveGrid {
  0% { background-position: 0 0, 0 0; }
  100% { background-position: 100px 100px, 100px 100px; }
}

/* FEATURE CARD */
.feature-card {
  background: rgba(255, 255, 255, 0.03);
  border: 1px solid rgba(255, 255, 255, 0.08);
  padding: 2.5rem;
  border-radius: 1.5rem;
  backdrop-filter: blur(12px);
  box-shadow: 0 0 20px rgba(46, 196, 182, 0.1);
  transition: all 0.4s ease;
  cursor: default;
}
.feature-card:hover {
  transform: translateY(-10px) scale(1.03);
  border-color: rgba(46, 196, 182, 0.7);
  box-shadow: 0 0 25px rgba(46, 196, 182, 0.4), 0 0 40px rgba(106, 60, 255, 0.3);
}

/* CARD ICON */
.icon-circle {
  width: 70px;
  height: 70px;
  border-radius: 50%;
  background: radial-gradient(circle, rgba(46,196,182,0.3), rgba(106,60,255,0.3));
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 2rem;
  color: white;
  margin-bottom: 1.5rem;
  transition: transform 0.4s ease;
}
.feature-card:hover .icon-circle {
  transform: scale(1.15) rotate(8deg);
}

/* TITLES */
.feature-title {
  font-size: 1.6rem;
  font-weight: 600;
  color: white;
  margin-bottom: 1rem;
}
.feature-text {
  color: #b9c7d7;
  line-height: 1.6;
}

/* NEON */
.neon-title {
  text-shadow: 0 0 10px #2EC4B6, 0 0 20px #2EC4B6;
}
</style>
