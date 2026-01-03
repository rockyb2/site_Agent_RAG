<template>
  <section id="agent" class="relative py-32 bg-[#050B19] overflow-hidden">
    <!-- Animated Grid Background -->
    <div class="absolute inset-0 grid-bg opacity-[0.07]"></div>

    <div class="relative z-10 max-w-7xl mx-auto px-6 md:px-12 lg:px-20">
      <!-- Titre principal -->
      <h2 class="text-center text-4xl md:text-6xl font-extrabold text-white mb-20 neon-title">
        Qu’est-ce qu’un Agent IA ?<br />
        <span class="text-3xl md:text-5xl text-[#2EC4B6]">L’avenir de votre entreprise</span>
      </h2>

      <!-- Introduction -->
      <div class="text-center max-w-4xl mx-auto mb-20">
        <p class="text-lg md:text-xl text-slate-300 leading-relaxed">
          Un Agent IA n’est pas un simple chatbot. C’est un <span class="highlight">collaborateur intelligent
            infatigable</span>
          capable de <strong>comprendre, raisonner, planifier et agir</strong> de manière autonome pour accomplir des
          tâches complexes.
          Il s’intègre à vos outils (emails, CRM, Excel, bases de données…) et travaille 24h/24 pour booster votre
          productivité.
        </p>
      </div>

      <!-- Grille principale : Définition + Pourquoi c’est indispensable -->
      <div class="grid lg:grid-cols-2 gap-12 mb-24">
        <!-- Définition -->
        <div class="agent-card reveal">
          <h3 class="agent-title">Définition simple et puissante</h3>
          <p class="agent-text">
            Un Agent IA va bien au-delà des réponses textuelles : il <span class="highlight">exécute des actions
              réelles</span>
            comme envoyer un email, générer un rapport Excel ou PDF, analyser des données, créer des tâches dans votre
            outil de gestion, etc.
          </p>
          <p class="agent-text mt-4">
            Alimenté par des modèles avancés (Grok, GPT, Claude…) et enrichi par le <strong>RAG</strong>, il connaît
            parfaitement
            vos documents internes et agit avec précision, sans hallucination.
          </p>
        </div>

        <!-- Pourquoi indispensable -->
        <div class="agent-card reveal">
          <h3 class="agent-title">Pourquoi votre entreprise en a besoin dès maintenant</h3>
          <ul class="agent-list space-y-4">
            <li>✔ Automatisation des tâches répétitives (gain de 20-40 % de temps)</li>
            <li>✔ Support client instantané et personnalisé 24/7</li>
            <li>✔ Réduction drastique des coûts opérationnels</li>
            <li>✔ Zéro fatigue : travaille sans pause ni erreur humaine</li>
            <li>✔ Libère vos équipes pour des missions créatives et stratégiques</li>
            <li>✔ Scalabilité infinie : un agent gère des milliers de tâches simultanément</li>
          </ul>
        </div>
      </div>

      <!-- Nouvelle section : Exemples concrets -->
      <h3 class="text-center text-3xl md:text-4xl font-bold text-white mb-16 neon-subtitle">
        Exemples concrets dans la vraie vie d’entreprise
      </h3>

      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-10">
        <!-- Exemple 1 -->
        <div class="example-card reveal">
          <div class="example-icon">📧</div>
          <h4 class="example-title">Gestion des demandes clients</h4>
          <p class="example-text">
            Un client envoie un email demandant un devis. L’Agent IA lit l’email, extrait les besoins, génère un devis
            Excel personnalisé,
            l’envoie automatiquement et crée une tâche dans votre CRM. Vos commerciaux gagnent des heures par jour.
          </p>
        </div>

        <!-- Exemple 2 -->
        <div class="example-card reveal">
          <div class="example-icon">📊</div>
          <h4 class="example-title">Reporting & Analyse</h4>
          <p class="example-text">
            Chaque lundi, l’Agent analyse vos ventes de la semaine, détecte les anomalies, crée un rapport PDF avec
            graphiques
            et l’envoie à la direction par email + Slack. Plus besoin d’attendre le rapport manuel.
          </p>
        </div>

        <!-- Exemple 3 -->
        <div class="example-card reveal">
          <div class="example-icon">🛠️</div>
          <h4 class="example-title">Support technique 24/7</h4>
          <p class="example-text">
            Un client pose une question technique à 2h du matin. L’Agent consulte votre base de connaissances interne
            (RAG),
            fournit une réponse précise et, si besoin, ouvre un ticket prioritaire. Satisfaction client explosée, équipe
            reposée.
          </p>
        </div>

        <!-- Exemple 4 -->
        <div class="example-card reveal">
          <div class="example-icon">👥</div>
          <h4 class="example-title">Ressources Humaines</h4>
          <p class="example-text">
            Onboarding automatisé : génération de contrat, planning de formations, réponses aux questions des nouveaux
            arrivants.
            Les RH se concentrent sur l’humain, pas sur la paperasse.
          </p>
        </div>

        <!-- Exemple 5 -->
        <div class="example-card reveal">
          <div class="example-icon">🚀</div>
          <h4 class="example-title">Marketing & Contenu</h4>
          <p class="example-text">
            L’Agent rédige des posts LinkedIn à partir de vos actualités internes, programme leur publication et analyse
            les performances.
            Votre visibilité augmente sans effort supplémentaire.
          </p>
        </div>

        <!-- Exemple 6 -->
        <div class="example-card reveal">
          <div class="example-icon">💡</div>
          <h4 class="example-title">Idées & Innovation</h4>
          <p class="example-text">
            Vous demandez : « Quelles améliorations pour notre produit ? » L’Agent analyse les retours clients, les
            données d’usage
            et propose 5 idées concrètes avec plan d’action. Vos brainstormings deviennent ultra-efficaces.
          </p>
        </div>
      </div>

      <!-- Conclusion + CTA -->
      <div class="text-center mt-24">
        <p class="text-xl md:text-2xl text-slate-200 mb-10 max-w-4xl mx-auto">
          Les Agents IA ne remplacent pas vos équipes.<br />
          <span class="text-[#2EC4B6] font-bold">Ils les rendent surhumaines.</span>
        </p>

        <a target="_blank" href="https://www.linkedin.com/in/jonathan-zadi-277824266" class="demo-btn">
          Réserver une démo personnalisée
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
  0% {
    background-position: 0 0;
  }

  100% {
    background-position: 120px 120px;
  }
}

/* Titres Neon */
.neon-title {
  text-shadow: 0 0 15px #2EC4B6, 0 0 30px #2EC4B6;
}

.neon-subtitle {
  text-shadow: 0 0 10px #2EC4B6, 0 0 20px #2EC4B6;
}

/* Cartes principales */
.agent-card {
  background: rgba(255, 255, 255, 0.03);
  border: 1px solid rgba(255, 255, 255, 0.07);
  padding: 2.5rem;
  border-radius: 1.5rem;
  backdrop-filter: blur(14px);
  box-shadow: 0 0 20px rgba(46, 196, 182, 0.09);
  transition: all 0.5s ease;
}

.agent-card:hover {
  transform: translateY(-12px) scale(1.03);
  border-color: #2EC4B6;
  box-shadow: 0 0 35px rgba(46, 196, 182, 0.4), 0 0 50px rgba(106, 60, 255, 0.3);
}

.agent-title {
  font-size: 2rem;
  font-weight: 700;
  color: white;
  margin-bottom: 1.5rem;
  text-shadow: 0 0 12px rgba(46, 196, 182, 0.6);
}

.agent-text {
  color: #b9c7d7;
  line-height: 1.8;
  font-size: 1.1rem;
}

.highlight {
  color: #2EC4B6;
  font-weight: 700;
}

.agent-list li {
  color: #d0e0f0;
  font-size: 1.1rem;
}

/* Cartes exemples */
.example-card {
  background: rgba(255, 255, 255, 0.04);
  border: 1px solid rgba(46, 196, 182, 0.2);
  padding: 2rem;
  border-radius: 1.5rem;
  text-align: center;
  transition: all 0.4s ease;
}

.example-card:hover {
  transform: translateY(-10px);
  background: rgba(46, 196, 182, 0.08);
  border-color: #2EC4B6;
}

.example-icon {
  font-size: 3.5rem;
  margin-bottom: 1rem;
}

.example-title {
  font-size: 1.5rem;
  font-weight: 600;
  color: white;
  margin-bottom: 1rem;
}

.example-text {
  color: #b9c7d7;
  line-height: 1.7;
  font-size: 1rem;
}

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