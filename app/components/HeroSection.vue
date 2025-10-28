<template>
  <section
    id="inicio"
    class="relative w-full min-h-[90vh] flex items-center overflow-hidden bg-cover bg-center bg-no-repeat"
    style="background-image: url('/imagens/Engenheiros de costas 1.png');"
    role="region"
    aria-label="Apresentação do site de Engenharia Civil"
  >
    <div class="absolute inset-0 bg-black/40" />

    <div class="relative z-10 w-full max-w-7xl mx-auto px-8 md:px-10 lg:px-16">
      <div class="max-w-xl">
        <h1 class="text-4xl md:text-4xl lg:text-4xl font-bold text-white leading-tight">
          Construindo Excelência, Transformando Projetos.
        </h1>
        <p class="mt-4 text-lg text-gray-200">
          Projetos de engenharia civil que transformam ideias em estruturas sólidas e duradouras.
        </p>

        <div class="mt-8">
          <a
            href="https://wa.me/message/MJHWYM756SHTA1"
            target="_blank"
            rel="noopener noreferrer"
            class="inline-block bg-orange-500 hover:bg-orange-400 text-black font-medium px-8 py-3 rounded-lg transition-colors duration-300"
          >
            Entre em contato conosco
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
section {
  background-size: cover;
  background-position: center center;
  image-rendering: -webkit-optimize-contrast;
}

a,
a:hover,
a:focus {
  color: #000 !important;
}
</style>
