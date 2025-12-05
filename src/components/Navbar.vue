<template>
  <header class="fixed inset-x-0 top-0 z-50 backdrop-blur-md bg-linear-to-r from-[#071026]/50 to-[#071026]/30 border-b border-white/5">
    <div class="max-w-7xl mx-auto px-6 md:px-12 lg:px-20 flex items-center justify-between h-16">
      <!-- Logo -->
      <a href="#" class="flex items-center gap-3">
        <span class="font-semibold text-lg text-white tracking-wide">Candide_AI</span>
      </a>

      <!-- Desktop nav -->
      <nav class="hidden lg:flex items-center gap-8 text-sm text-slate-200">
        <a href="#creations" class="hover:text-white/90 transition">Creations</a>
        <a href="#rag" class="hover:text-white/90 transition">RAG</a>
        <a href="#agent" class="hover:text-white/90 transition">Agent IA</a>
        <a href="#comparatif" class="hover:text-white/90 transition">Comparatif</a>
        <a href="#about" class="hover:text-white/90 transition">About</a>
        <a href="#contact" class="hover:text-white/90 transition">Contact</a>
      </nav>

      <!-- Actions / Mobile button -->
      <div class="flex items-center gap-3">
        <button class="hidden lg:inline-flex items-center gap-2 px-5 py-2 rounded-lg bg-linear-to-r from-[#6A3CFF] to-[#2EC4B6] text-white font-medium hover:brightness-105 active:scale-95 transition">
          Get started
        </button>

        <button @click="open = !open" aria-label="Open menu" class="lg:hidden p-2 rounded-md text-white/90 hover:bg-white/5 transition">
          <svg v-if="!open" xmlns="http://www.w3.org/2000/svg" width="26" height="26" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round">
            <path d="M3 7h18M3 12h18M3 17h18"></path>
          </svg>
          <svg v-else xmlns="http://www.w3.org/2000/svg" width="26" height="26" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round">
            <path d="M18 6L6 18M6 6l12 12"></path>
          </svg>
        </button>
      </div>
    </div>

    <!-- Mobile menu overlay -->
    <transition name="menu-fade">
      <div v-if="open" class="lg:hidden fixed inset-0 z-40 bg-black/60 backdrop-blur-sm flex items-center justify-center">
        <div class="bg-[#071026]/95 rounded-2xl w-11/12 max-w-md p-6 border border-white/5 shadow-2xl">
          <div class="flex flex-col gap-6 text-lg text-slate-100">
            <a @click="close" href="#creations" class="block hover:text-white/90 transition">Creations</a>
            <a @click="close" href="#rag" class="block hover:text-white/90 transition">RAG</a>
            <a @click="close" href="#agent" class="block hover:text-white/90 transition">Agent IA</a>
            <a @click="close" href="#comparatif" class="block hover:text-white/90 transition">Comparatif</a>
            <a @click="close" href="#about" class="block hover:text-white/90 transition">About</a>
            <a @click="close" href="#contact" class="block hover:text-white/90 transition">Contact</a>
          </div>
          <div class="mt-6 flex justify-center">
            <button @click="close" class="px-6 py-2 rounded-full bg-linear-to-r from-[#6A3CFF] to-[#2EC4B6] text-white font-medium">Book demo</button>
          </div>
        </div>
      </div>
    </transition>

  </header>
</template>

<script setup>
import { ref } from 'vue'
const open = ref(false)
function close(){ open.value = false }
</script>

<style scoped>
.menu-fade-enter-active, .menu-fade-leave-active { transition: opacity 240ms ease; }
.menu-fade-enter-from, .menu-fade-leave-to { opacity: 0; }
.menu-fade-enter-to, .menu-fade-leave-from { opacity: 1; }
</style>
