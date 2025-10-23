<template>
  <!-- Hero Section responsiva com imagem de fundo e texto centralizado à esquerda -->
  <section
    class="relative w-full min-h-[80vh] flex items-center overflow-hidden"
    role="region"
    aria-label="Apresentação do site de Engenharia Civil"
  >
    <!-- Imagem de fundo -->
    <img
      src=""
      alt="Imagem de fundo de engenharia civil"
      class="absolute inset-0 w-full h-full object-cover object-center"
      loading="lazy"
    />

    <!-- Sobreposição para contraste -->
    <div class="absolute inset-0 bg-black/40"></div>

    <!-- Conteúdo -->
    <div class="relative z-10 w-full max-w-6xl mx-auto px-6 md:px-10 lg:px-16">
      <div class="max-w-xl">
        <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-white leading-tight">
          Construindo o futuro com excelência e segurança.
        </h1>
        <p class="mt-4 text-lg text-gray-200">
          Projetos de engenharia civil que transformam ideias em estruturas sólidas e duradouras.
        </p>

        <!-- Botão de contato -->
        <div class="mt-8">
          <nuxt-link
            to="/contatos"
            class="inline-block bg-orange-500 hover:bg-orange-600 text-white font-semibold px-6 py-3 rounded-lg transition-colors duration-300 shadow-md"
          >
            Entre em contato conosco
          </nuxt-link>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
// HeroSection - componente para página inicial de Engenharia Civil
</script>

<style scoped>
@media (max-width: 640px) {
  h1 {
    line-height: 1.1;
  }
}
</style>
