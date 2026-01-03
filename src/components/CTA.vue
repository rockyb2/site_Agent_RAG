<template>
  <section id="contact" class="relative py-40 overflow-hidden bg-[#050B19] text-center">

    <!-- Futuristic Grid Background -->
    <div class="absolute inset-0 grid-bg opacity-[0.08]"></div>

    <!-- Neon glow halo -->
    <div class="absolute -top-40 left-1/2 -translate-x-1/2 w-[600px] h-[600px] bg-[#2EC4B6]/20 blur-[150px] rounded-full"></div>

    <div class="relative z-10 max-w-4xl mx-auto px-6">

      <h2 class="text-4xl md:text-6xl font-extrabold text-white mb-8 neon-strong">
        Transformez votre entreprise dès aujourd’hui
      </h2>

      <p class="text-lg md:text-xl text-slate-300 max-w-2xl mx-auto mb-14 animate-fade">
        Découvrez comment un agent IA alimenté par le RAG peut automatiser vos processus,
        booster votre productivité et réduire vos coûts opérationnels.
      </p>

      <button class="cta-btn">
       <a target="_blank" href="https://www.linkedin.com/in/jonathan-zadi-277824266" >Réserver une démo</a> 
      </button>

    </div>
  </section>
</template>

<script setup>
import { onMounted } from 'vue'
import gsap from 'gsap'

onMounted(() => {
  gsap.from('.neon-strong', { opacity: 0, y: 40, duration: 1.2 })
  gsap.from('.animate-fade', { opacity: 0, y: 25, delay: 0.3, duration: 1.2 })
  gsap.from('.cta-btn', { opacity: 0, scale: 0.8, delay: 0.6, duration: 1.1 })
})
</script>

<style scoped>
/* Grid Background */
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

/* Neon Strong Title */
.neon-strong {
  text-shadow: 0 0 10px #2EC4B6, 0 0 25px #2EC4B6, 0 0 45px #2EC4B6;
}

/* Fade Animation */
@keyframes fadeUp {
  0% { opacity: 0; transform: translateY(20px); }
  100% { opacity: 1; transform: translateY(0); }
}
.animate-fade {
  animation: fadeUp 1s ease forwards;
}

/* CTA Button */
.cta-btn {
  display: inline-block;
  padding: 1.1rem 3rem;
  font-size: 1.3rem;
  font-weight: 600;
  color: white;
  border-radius: 1rem;
  background: linear-gradient(90deg, #2EC4B6, #6A3CFF);
  box-shadow: 0 0 20px rgba(46,196,182,0.4), 0 0 35px rgba(106,60,255,0.3);
  
  cursor: pointer;
}
.cta-btn:hover {
  transform: scale(1.06);
  box-shadow: 0 0 30px rgba(46,196,182,0.6), 0 0 55px rgba(106,60,255,0.5);
}
.cta-btn:active {
  transform: scale(0.96);
}
</style>
