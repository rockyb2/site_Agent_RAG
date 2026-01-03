<template>
    <section id="demo" class="relative py-32 bg-[#050B19] text-white overflow-hidden">

        <!-- Grid Background -->
        <div class="absolute inset-0 grid-bg opacity-[0.06]"></div>

        <!-- Glow Halo -->
        <div
            class="absolute top-0 left-1/2 -translate-x-1/2 w-[650px] h-[650px] bg-[#2EC4B6]/15 blur-[180px] rounded-full">
        </div>

        <div class="relative z-10 max-w-6xl mx-auto px-6 text-center">

            <!-- Title -->
            <h2 class="text-4xl md:text-6xl font-extrabold neon-strong mb-8">
                Testez Nos Agents IA en Direct
            </h2>

            <p class="max-w-3xl mx-auto text-slate-300 text-lg md:text-xl mb-16 animate-fade">
                Testez notre agent de type chatbot, doté d’outils lui permettant de générer des fichiers Word, Excel et PDF, puis de les envoyer par e-mail.
            </p>

            <!-- Cards -->
            <div class="grid md:grid-cols-2 gap-12 max-w-6xl mx-auto">

                <!-- Agent Financier IA
                <div
                    class="p-10 rounded-2xl bg-white/10 backdrop-blur-xl border border-[#2EC4B6]/20 shadow-xl hover:shadow-[#2EC4B6]/40 transition transform hover:-translate-y-2">
                    <h3 class="text-3xl font-semibold text-[#2EC4B6] mb-4">Agent Financier IA</h3>
                    <p class="text-gray-300 leading-relaxed mb-6">
                        Analyse financière intelligente : prévisions, risques, investissements, stratégies
                        d’optimisation.
                    </p>
                    <iframe src="https://5e3a364796be067d68.gradio.live"
                        class="w-full h-[500px] rounded-xl border border-[#2EC4B6]/30"></iframe>
                </div>

                <!-- Agent Communal RAG -->
                <!-- <div
                    class="p-10 rounded-2xl bg-white/10 backdrop-blur-xl border border-[#2EC4B6]/20 shadow-xl hover:shadow-[#2EC4B6]/40 transition transform hover:-translate-y-2">
                    <h3 class="text-3xl font-semibold text-[#2EC4B6] mb-4">Agent Communal RAG</h3>
                    <p class="text-gray-300 leading-relaxed mb-6">
                        L’agent officiel de la commune fictive <span
                            class="text-[#FF9F1C] font-bold">Trifouillis‑sur‑Loire</span>, capable de répondre aux
                        documents municipaux.
                    </p>
                    <iframe src="https://b83bb0f415730ddfc9.gradio.live"
                        class="w-full h-[500px] rounded-xl border border-[#2EC4B6]/30"></iframe>
                </div> -->

            </div>

            <!-- RAG Commune Agent Card -->
            <!-- <div class="card mt-10">
                <h3 class="text-3xl font-bold mb-4 text-[#FF9F1C]">Agent IA avec RAG – Trifouillis‑sur‑Loire</h3>
                <p class="text-slate-300 mb-6 text-sm leading-relaxed">
                    Cet agent utilise vos documents internes pour fournir des réponses fiables.
                    Ici, il gère une commune fictive en accédant automatiquement aux informations locales.
                </p>
                <a href="https://b83bb0f415730ddfc9.gradio.live" target="_blank" class="demo-btn">
                    Tester l’Agent RAG
                </a>
            </div> -->

            <!-- <div class="card mt-10">
                <h3 class="text-3xl font-bold mb-4 text-[#FF9F1C]">Agent IA expert en finance</h3>
                <p class="text-slate-300 mb-6 text-sm leading-relaxed">
                    Cet Agent utilise des outils spécialement coder pour la finance vous pouvez lui poser des questions sur la valeur d'une action par exemple
                </p>
                <a href="https://5e3a364796be067d68.gradio.live" target="_blank" class="demo-btn">
                    Tester l’Agent Financier
                </a>
            </div> -->

            <div class="card mt-10">
                <h3 class="text-3xl font-bold mb-4 text-[#FF9F1C]">Candide Agent support</h3>
                <p class="text-slate-300 mb-6 text-sm leading-relaxed">
                    Un agent IA de support client capable de générer et d’envoyer des documents (Word, Excel, PDF) par e-mail.
                </p>
                <a href="https://chatbot-ui-6fre.onrender.com/" target="_blank" class="demo-btn">
                    Tester l’Agent Support
                </a>
            </div>
        </div>

        
    </section>
</template>

<script setup>
import { onMounted } from 'vue'
import gsap from 'gsap'
import ScrollReveal from 'scrollreveal'

onMounted(() => {
    gsap.from('.neon-strong', { opacity: 0, y: 40, duration: 1.2 })
    gsap.from('.animate-fade', { opacity: 0, y: 25, delay: 0.3, duration: 1.2 })

    ScrollReveal().reveal('.card', {
        duration: 1200,
        distance: '40px',
        origin: 'bottom',
        interval: 200,
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
        background-position: 0 0, 0 0;
    }

    100% {
        background-position: 120px 120px, 120px 120px;
    }
}

/* Neon Title */
.neon-strong {
    text-shadow: 0 0 10px #2EC4B6, 0 0 25px #2EC4B6, 0 0 45px #2EC4B6;
}

/* Fade Animation */
@keyframes fadeUp {
    0% {
        opacity: 0;
        transform: translateY(20px);
    }

    100% {
        opacity: 1;
        transform: translateY(0);
    }
}

.animate-fade {
    animation: fadeUp 1s ease forwards;
}

/* Card Style */
.card {
    background: rgba(255, 255, 255, 0.05);
    padding: 2.5rem;
    border-radius: 1.5rem;
    border: 1px solid rgba(255, 255, 255, 0.12);
    box-shadow: 0 0 25px rgba(0, 0, 0, 0.45);
    backdrop-filter: blur(10px);
    transition: all 0.35s ease;
}

.card:hover {
    transform: translateY(-6px) scale(1.02);
    box-shadow: 0 0 35px rgba(46, 196, 182, 0.3), 0 0 60px rgba(106, 60, 255, 0.25);
}

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
