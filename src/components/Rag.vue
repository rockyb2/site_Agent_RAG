<template>
  <section id="rag" class="relative py-32 bg-[#050B19] overflow-hidden">
    <!-- Animated Grid Background -->
    <div class="absolute inset-0 grid-bg opacity-[0.07]"></div>

    <div class="relative z-10 max-w-7xl mx-auto px-6 md:px-12 lg:px-20">
      <!-- Titre principal -->
      <h2 class="text-center text-4xl md:text-6xl font-extrabold text-white mb-20 neon-title">
        Qu’est-ce que le RAG ?<br />
        <span class="text-3xl md:text-5xl text-[#2EC4B6]">La clé pour une IA fiable et intelligente</span>
      </h2>

      <!-- Introduction avec analogie -->
      <div class="text-center max-w-4xl mx-auto mb-20">
        <p class="text-lg md:text-xl text-slate-300 leading-relaxed mb-8">
          Imaginez un bibliothécaire ultra-efficace dans une immense bibliothèque (vos documents d’entreprise : PDF, emails, fiches produits, contrats…).
          Quand vous posez une question, il ne devine pas la réponse : il <strong>va chercher les bons livres</strong>, lit les pages pertinentes,
          et vous donne une réponse précise et vérifiée.
        </p>
        <p class="text-lg md:text-xl text-slate-300 leading-relaxed">
          C’est exactement ce que fait le <strong>RAG (Retrieval-Augmented Generation)</strong> : l’IA <span class="highlight">cherche d’abord les infos dans VOS données internes</span>,
          puis génère une réponse fiable. Fini les réponses inventées ou génériques !
        </p>
      </div>

      <!-- Diagramme simple (placeholder image) -->
      <div class="flex justify-center mb-20">
        <div class="rag-diagram reveal">
          <img src="https://miro.medium.com/1*w5dEDJrGGmmZomPkMGpBsg.png" alt="Schéma simple du RAG : Question → Recherche dans documents → Réponse fiable" class="rounded-2xl shadow-2xl max-w-full h-auto" />
          <p class="text-center text-slate-400 mt-4 text-sm">Schéma simple : l’IA cherche avant de répondre</p>
        </div>
      </div>

      <!-- Comment ça marche en 3 étapes simples -->
      <h3 class="text-center text-3xl md:text-4xl font-bold text-white mb-16 neon-subtitle">
        Comment ça marche ? En 3 étapes ultra-simples
      </h3>

      <div class="grid md:grid-cols-3 gap-10 mb-24">
        <div class="step-card reveal">
          <div class="step-number">1</div>
          <h4 class="step-title">Vous posez une question</h4>
          <p class="step-text">Exemple : "Quelle est notre politique de retour pour les clients ?"</p>
        </div>
        <div class="step-card reveal">
          <div class="step-number">2</div>
          <h4 class="step-title">L’IA cherche dans VOS documents</h4>
          <p class="step-text">Elle fouille automatiquement vos PDF, emails, bases de données… et trouve les infos exactes.</p>
        </div>
        <div class="step-card reveal">
          <div class="step-number">3</div>
          <h4 class="step-title">Elle répond avec précision</h4>
          <p class="step-text">Réponse fiable, basée sur vos données réelles, sans invention ni erreur.</p>
        </div>
      </div>

      <!-- Exemples concrets en entreprise -->
      <h3 class="text-center text-3xl md:text-4xl font-bold text-white mb-16 neon-subtitle">
        Exemples concrets dans votre entreprise
      </h3>

      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-10">
        <!-- Exemple 1 -->
        <div class="example-card reveal">
          <div class="example-icon">🛒</div>
          <h4 class="example-title">Support client ultra-rapide</h4>
          <p class="example-text">
            Un client demande : "Mon produit est en retard, que faire ?"<br />
            L’IA RAG cherche dans vos procédures internes et répond immédiatement avec la bonne solution. Vos équipes support gagnent des heures et les clients sont plus satisfaits.
          </p>
        </div>

        <!-- Exemple 2 -->
        <div class="example-card reveal">
          <div class="example-icon">📊</div>
          <h4 class="example-title">Ventes & Devis</h4>
          <p class="example-text">
            Un commercial demande : "Quel prix pour ce client premium ?"<br />
            L’IA trouve les tarifs spéciaux dans vos contrats et propose un devis précis. Plus de recherches manuelles = plus de ventes closes rapidement.
          </p>
        </div>

        <!-- Exemple 3 -->
        <div class="example-card reveal">
          <div class="example-icon">👥</div>
          <h4 class="example-title">RH & Onboarding</h4>
          <p class="example-text">
            Nouveau salarié : "Combien de jours de congé me reste-t-il ?"<br />
            L’IA consulte le dossier RH et répond instantanément. Les RH se concentrent sur l’humain, pas sur les questions répétitives.
          </p>
        </div>

        <!-- Exemple 4 -->
        <div class="example-card reveal">
          <div class="example-icon">📄</div>
          <h4 class="example-title">Analyse de documents</h4>
          <p class="example-text">
            Vous demandez un résumé d’un contrat de 50 pages.<br />
            L’IA lit tout, extrait les points clés et vous donne un résumé clair. Gain de temps énorme pour les juristes ou managers.
          </p>
        </div>

        <!-- Exemple 5 -->
        <div class="example-card reveal">
          <div class="example-icon">🛡️</div>
          <h4 class="example-title">Conformité & Réglementation</h4>
          <p class="example-text">
            "Quelles sont les nouvelles règles RGPD ?"<br />
            L’IA cherche dans vos documents légaux à jour et explique simplement. Moins de risques d’erreur et plus de sérénité.
          </p>
        </div>

        <!-- Exemple 6 -->
        <div class="example-card reveal">
          <div class="example-icon">💡</div>
          <h4 class="example-title">Formation interne</h4>
          <p class="example-text">
            Un employé demande comment utiliser un outil interne.<br />
            L’IA trouve le tutoriel exact et l’explique pas à pas. Tout le monde monte en compétence plus vite.
          </p>
        </div>
      </div>

      <!-- Bénéfices pour les conditions de travail -->
      <div class="benefits-section text-center mt-24 max-w-4xl mx-auto">
        <h3 class="text-3xl md:text-4xl font-bold text-white mb-10 neon-subtitle">
          Comment le RAG améliore la vie au travail
        </h3>
        <p class="text-xl text-slate-200 mb-8">
          Moins de tâches répétitives → Moins de stress → Plus de temps pour le vrai travail créatif et stratégique.<br />
          <span class="text-[#2EC4B6] font-bold">Vos équipes deviennent plus efficaces, plus motivées et plus heureuses !</span>
        </p>
        <ul class="text-left max-w-2xl mx-auto text-lg text-slate-300 space-y-4">
          <li>✔ Gain de temps énorme (jusqu’à 30-50% sur les recherches d’info)</li>
          <li>✔ Réduction des erreurs et frustrations</li>
          <li>✔ Meilleure collaboration (tout le monde a les bonnes infos instantanément)</li>
          <li>✔ Scalable : fonctionne pour 10 ou 1000 employés sans effort supplémentaire</li>
        </ul>
      </div>

      <!-- CTA final -->
      <div class="text-center mt-24">
       
          <a target="_blank" href="https://www.linkedin.com/in/jonathan-zadi-277824266" class="demo-btn">
            Réserver une démo pour voir le RAG en action dans VOTRE entreprise
          </a>
        
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
    distance: '50px',
    origin: 'bottom',
    interval: 200,
    easing: 'ease-out'
  })
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
  0% { background-position: 0 0; }
  100% { background-position: 120px 120px; }
}

/* Neon Titles */
.neon-title { text-shadow: 0 0 15px #2EC4B6, 0 0 30px #2EC4B6; }
.neon-subtitle { text-shadow: 0 0 10px #2EC4B6, 0 0 20px #2EC4B6; }

/* Highlight */
.highlight { color: #2EC4B6; font-weight: 700; }

/* Étapes */
.step-card {
  background: rgba(255,255,255,0.04);
  border: 1px solid rgba(46,196,182,0.3);
  padding: 2rem;
  border-radius: 1.5rem;
  text-align: center;
  transition: all 0.4s ease;
}
.step-card:hover { transform: translateY(-10px); border-color: #2EC4B6; }
.step-number {
  font-size: 4rem;
  font-weight: bold;
  color: #2EC4B6;
  margin-bottom: 1rem;
}
.step-title { font-size: 1.6rem; color: white; margin-bottom: 1rem; }
.step-text { color: #b9c7d7; line-height: 1.6; }
/* Exemples */
.example-card {
  background: rgba(255,255,255,0.04);
  border: 1px solid rgba(46,196,182,0.2);
  padding: 2rem;
  border-radius: 1.5rem;
  text-align: center;
  transition: all 0.4s ease;
}
.example-card:hover { transform: translateY(-10px); background: rgba(46,196,182,0.08); border-color: #2EC4B6; }
.example-icon { font-size: 3.5rem; margin-bottom: 1rem; }
.example-title { font-size: 1.5rem; color: white; margin-bottom: 1rem; }
.example-text { color: #b9c7d7; line-height: 1.6; }

/* Diagramme */
.rag-diagram { max-width: 800px; }

/* Demo Buttons */
.demo-btn {
    display: inline-block;
    padding: 0.9rem 2.5rem;
    border-radius: 1rem;
    background: linear-gradient(90deg, #2EC4B6, #6A3CFF);
    font-weight: 600;
    color: white;
    transition: all 0.3s ease;
    box-shadow: 0 0 20px rgba(46, 196, 182, 0.4);
}

.demo-btn:hover {
    transform: scale(1.05);
    box-shadow: 0 0 35px rgba(46, 196, 182, 0.6), 0 0 55px rgba(106, 60, 255, 0.5);
}
</style>