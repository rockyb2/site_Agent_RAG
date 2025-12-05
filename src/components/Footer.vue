<template>
  <footer class="relative bg-[#050B19] text-white py-20 overflow-hidden">

    <!-- Grid Background -->
    <div class="absolute inset-0 grid-bg opacity-[0.06]"></div>

    <!-- Glow Circles -->
    <div class="absolute -bottom-32 -left-20 w-[500px] h-[500px] bg-[#2EC4B6]/20 blur-[180px] rounded-full"></div>
    <div class="absolute -top-20 -right-10 w-[450px] h-[450px] bg-[#6A3CFF]/20 blur-[180px] rounded-full"></div>

    <div class="relative z-10 max-w-6xl mx-auto px-6">

      <div class="grid md:grid-cols-4 gap-12 border-b border-white/10 pb-12">

        <!-- Brand -->
        <div>
          <h2 class="text-3xl font-extrabold neon-strong mb-4">Candide_AI</h2>
          <p class="text-slate-300 text-sm leading-relaxed">
            La solution d'agent IA alimenté par RAG pour transformer vos processus,
            automatiser vos tâches et booster votre croissance.
          </p>
        </div>

        <!-- Menu -->
        <div>
          <h3 class="text-lg font-semibold mb-4 text-[#2EC4B6]">Navigation</h3>
          <ul class="space-y-2 text-slate-300">
            <li><a href="#rag" class="hover:text-[#2EC4B6] transition">RAG</a></li>
            <li><a href="#agent" class="hover:text-[#2EC4B6] transition">Agent IA</a></li>
            <li><a href="#comparatif" class="hover:text-[#2EC4B6] transition">Comparatif</a></li>
            <li><a href="#cta" class="hover:text-[#2EC4B6] transition">Demande de Démo</a></li>
          </ul>
        </div>

        <!-- Contact -->
        <div>
          <h3 class="text-lg font-semibold mb-4 text-[#2EC4B6]">Contact</h3>
          <ul class="space-y-2 text-slate-300 text-sm">
            <li>Email : rockyb225.dev@gmail.com</li>
            <li>Téléphone : +225 05 64 21 85 67</li>
            <li>Adresse : Riviera Palmeraie, Côte D'ivoire</li>
          </ul>
        </div>

        <!-- Social -->
        <div>
          <h3 class="text-lg font-semibold mb-4 text-[#2EC4B6]">Réseaux</h3>
          <div class="flex space-x-4 text-2xl">
            <a target="_blank" href="https://www.linkedin.com/in/jonathan-zadi-277824266" class="hover:text-[#2EC4B6] text-white transition"><i class="fa-brands fa-linkedin"></i></a>
            <a target="_blank" href="https://www.facebook.com/profile.php?id=61582837157806" class="hover:text-[#2EC4B6] transition"><i class="fa-brands fa-square-facebook"></i></a>
            
          </div>
        </div>

      </div>

      <!-- Bottom -->
      <div class="text-center text-slate-400 text-sm pt-8">
        © {{ new Date().getFullYear() }} Candide_AI — Tous droits réservés.
      </div>

    </div>
  </footer>
</template>

<script setup>
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

/* Neon Strong Brand */
.neon-strong {
  text-shadow: 0 0 8px #2EC4B6, 0 0 20px #2EC4B6;
}
</style>
