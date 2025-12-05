<template>
  <section id="hero" class="relative min-h-screen flex items-center justify-center overflow-hidden bg-[#050B19] pt-24">

    <!-- Animated Grid Background -->
    <div class="absolute inset-0 opacity-[0.15] grid-bg pointer-events-none"></div>

    <!-- Particles Canvas -->
    <canvas id="particles" class="absolute inset-0 pointer-events-none"></canvas>

    <!-- Hologram 3D -->
    <div class="relative z-10 flex flex-col items-center text-center px-6">
      <div class="holo-wrapper mb-10">
        <div class="holo-core"></div>
        <div class="holo-ring"></div>
      </div>

      <h1 class="text-4xl md:text-6xl font-extrabold text-white mb-6 neon-title">
        Boostez votre entreprise avec un Agent IA intelligent
      </h1>

      <p class="text-lg md:text-xl text-slate-300 max-w-2xl mb-10 animate-fade-in">
        Un agent IA alimenté par la technologie RAG, capable de comprendre vos données internes,
        exécuter des actions et automatiser vos processus.
      </p>

      <button class="px-10 py-4 cursor-pointer text-lg rounded-xl bg-linear-to-r from-[#2EC4B6] to-[#6A3CFF] text-white font-semibold shadow-lg hover:shadow-2xl hover:scale-[1.04]  transition">
        Demander une démo
      </button>
    </div>

  </section>
</template>

<script setup>
import { onMounted } from 'vue'
import gsap from 'gsap'

onMounted(() => {
  // GSAP hero animations
  gsap.from('.neon-title', { opacity: 0, y: 40, duration: 1.2 })
  gsap.from('.animate-fade-in', { opacity: 0, y: 30, delay: 0.4, duration: 1.2 })
  gsap.from('button', { opacity: 0, y: 30, delay: 0.7, duration: 1.2 })

  // Particles Effect
  const canvas = document.getElementById('particles')
  const ctx = canvas.getContext('2d')
  let particles = []

  canvas.width = window.innerWidth
  canvas.height = window.innerHeight

  const createParticles = () => {
    for (let i = 0; i < 80; i++) {
      particles.push({
        x: Math.random() * canvas.width,
        y: Math.random() * canvas.height,
        size: Math.random() * 2 + 1,
        speedX: (Math.random() - 0.5) * 0.6,
        speedY: (Math.random() - 0.5) * 0.6
      })
    }
  }

  const animateParticles = () => {
    ctx.clearRect(0, 0, canvas.width, canvas.height)

    particles.forEach(p => {
      p.x += p.speedX
      p.y += p.speedY

      if (p.x < 0 || p.x > canvas.width) p.speedX *= -1
      if (p.y < 0 || p.y > canvas.height) p.speedY *= -1

      ctx.fillStyle = 'rgba(46, 196, 182, 0.7)'
      ctx.beginPath()
      ctx.arc(p.x, p.y, p.size, 0, Math.PI * 2)
      ctx.fill()
    })

    requestAnimationFrame(animateParticles)
  }

  createParticles()
  animateParticles()
})
</script>

<style scoped>
/* Futuristic animated grid */
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

/* Hologram 3D */
.holo-wrapper {
  width: 210px;
  height: 210px;
  perspective: 900px;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
}
.holo-core {
  width: 130px;
  height: 130px;
  background: radial-gradient(circle, rgba(46,196,182,0.45), rgba(106,60,255,0.4));
  border-radius: 50%;
  filter: blur(18px);
  animation: holoSpin 6s linear infinite;
}

.holo-ring {
  position: absolute;
  width: 200px;
  height: 200px;
  border-radius: 50%;
  border: 2px solid rgba(255,255,255,0.15);
  animation: ringRotate 9s linear infinite;
}

@keyframes holoSpin {
  from { transform: rotateX(0) rotateY(0); }
  to { transform: rotateX(360deg) rotateY(360deg); }
}

@keyframes ringRotate {
  from { transform: rotateZ(0); }
  to { transform: rotateZ(360deg); }
}

/* Neon Title */
.neon-title {
  text-shadow: 0 0 10px #2EC4B6, 0 0 25px #2EC4B6, 0 0 40px #2EC4B6;
}

/* Fade animations */
@keyframes fadeInUp {
  0% { opacity: 0; transform: translateY(20px); }
  100% { opacity: 1; transform: translateY(0); }
}
.animate-fade-in { animation: fadeInUp 1.2s ease forwards; }
</style>
