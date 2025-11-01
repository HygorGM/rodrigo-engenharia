<template>
  <header
    :class="[
      'fixed top-0 left-0 w-full bg-white/90 backdrop-blur-md shadow-sm z-50 transition-transform duration-500',
      isVisible ? 'translate-y-0' : '-translate-y-full'
    ]"
  >
    <div class="max-w-7xl mx-auto flex justify-between items-center px-6 py-4">
      <div class="flex items-center">
        <img
          src="/imagens/Logo.png"
          alt="Logo da empresa"
          class="w-20 h-auto object-contain"
        >
      </div>

      <nav class="hidden md:flex items-center space-x-6 text-gray-900 font-medium">
        <a href="#inicio" class="hover:text-orange-500 transition">Início</a>
        <a href="#sobre" class="hover:text-orange-500 transition">Sobre</a>
        <a href="#servicos" class="hover:text-orange-500 transition">Serviços</a>
        <a href="#portifolio" class="hover:text-orange-500 transition">Portfólio</a>
        <a href="#contatos" class="hover:text-orange-500 transition">Contato</a>
      </nav>

      <button
        class="md:hidden text-gray-900 focus:outline-none"
        @click="toggleMenu"
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
          <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16" />
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
          <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
        </svg>
      </button>
    </div>

    <transition name="slide">
      <div
        v-if="isOpen"
        class="md:hidden bg-white shadow-inner px-6 py-8 text-gray-900 font-medium flex flex-col items-center justify-center space-y-4 text-center"
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
import { ref, onMounted, onUnmounted } from 'vue'

const isOpen = ref(false)
const isVisible = ref(true)
let lastScroll = 0

const toggleMenu = () => (isOpen.value = !isOpen.value)
const closeMenu = () => (isOpen.value = false)

const handleScroll = () => {
  const currentScroll = window.scrollY
  if (currentScroll <= 0) {
    isVisible.value = true
  } else if (currentScroll > lastScroll) {
    isVisible.value = false
  } else {
    isVisible.value = true
  }
  lastScroll = currentScroll
}

onMounted(() => window.addEventListener('scroll', handleScroll))
onUnmounted(() => window.removeEventListener('scroll', handleScroll))
</script>

<style scoped>
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
