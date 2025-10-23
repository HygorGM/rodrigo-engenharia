<template>
  <header
    class="fixed top-0 left-0 w-full bg-white/90 backdrop-blur-md shadow-sm z-50 transition-all duration-300"
  >
    <div
      class="max-w-7xl mx-auto flex justify-between items-center px-6 py-4"
    >
      <!-- Logo -->
      <div class="flex items-center">
        <img
          src=""
          alt="Logo da empresa"
          class="w-14 h-auto object-contain"
        />
      </div>

      <!-- Menu desktop -->
      <nav class="hidden md:flex items-center space-x-6 text-gray-900 font-medium">
        <a href="#hero" class="hover:text-orange-500 transition">Início</a>
        <a href="#sobre" class="hover:text-orange-500 transition">Sobre</a>
        <a href="#objetivo" class="hover:text-orange-500 transition">Objetivos</a>
        <a href="#valores" class="hover:text-orange-500 transition">Valores</a>
        <a href="#servicos" class="hover:text-orange-500 transition">Serviços</a>
        <a href="#portifolio" class="hover:text-orange-500 transition">Portfólio</a>
        <a href="#contato" class="hover:text-orange-500 transition">Contato</a>
      </nav>

      <!-- Ícone menu mobile -->
      <button
        @click="toggleMenu"
        class="md:hidden text-gray-900 focus:outline-none"
      >
        <svg
          v-if="!isOpen"
          xmlns="http://www.w3.org/2000/svg"
          class="h-7 w-7"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path stroke-linecap="round" stroke-linejoin="round"
            d="M4 6h16M4 12h16M4 18h16" />
        </svg>
        <svg
          v-else
          xmlns="http://www.w3.org/2000/svg"
          class="h-7 w-7"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path stroke-linecap="round" stroke-linejoin="round"
            d="M6 18L18 6M6 6l12 12" />
        </svg>
      </button>
    </div>

    <!-- Menu mobile (dropdown com animação suave) -->
    <transition name="slide">
      <div
        v-if="isOpen"
        class="md:hidden bg-white shadow-inner px-6 py-4 text-gray-900 font-medium space-y-4"
      >
        <a href="#hero" class="block hover:text-orange-500" @click="closeMenu">Início</a>
        <a href="#sobre" class="block hover:text-orange-500" @click="closeMenu">Sobre</a>
        <a href="#objetivo" class="block hover:text-orange-500" @click="closeMenu">Objetivos</a>
        <a href="#valores" class="block hover:text-orange-500" @click="closeMenu">Valores</a>
        <a href="#servicos" class="block hover:text-orange-500" @click="closeMenu">Serviços</a>
        <a href="#portifolio" class="block hover:text-orange-500" @click="closeMenu">Portfólio</a>
        <a href="#contato" class="block hover:text-orange-500" @click="closeMenu">Contato</a>
      </div>
    </transition>
  </header>
</template>

<script setup>
import { ref } from 'vue'

const isOpen = ref(false)
const toggleMenu = () => (isOpen.value = !isOpen.value)
const closeMenu = () => (isOpen.value = false)
</script>

<style scoped>
/* Animação suave do dropdown mobile */
.slide-enter-active,
.slide-leave-active {
  transition: all 0.3s ease;
  overflow: hidden;
}

.slide-enter-from {
  max-height: 0;
  opacity: 0;
}

.slide-enter-to {
  max-height: 500px;
  opacity: 1;
}

.slide-leave-from {
  max-height: 500px;
  opacity: 1;
}

.slide-leave-to {
  max-height: 0;
  opacity: 0;
}
</style>
