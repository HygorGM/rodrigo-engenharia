<template>
  <section
    id="inicio"
    class="relative w-full flex items-center justify-center overflow-hidden"
    role="region"
    aria-label="Apresentação do site de Engenharia Civil"
  >
    <!-- Imagem de fundo -->
    <img
      src="/imagens/Engenheiros de costas 1.png"
      alt="Engenheiros de costas"
      class="absolute inset-0 w-full h-full object-cover"
    />

    <!-- Camada de escurecimento -->
    <div class="absolute inset-0 bg-black/40"></div>

    <!-- Conteúdo principal -->
    <div
      class="relative z-10 w-full max-w-7xl mx-auto px-8 md:px-10 lg:px-16 flex items-center min-h-[calc(100vh-5rem)]"
    >
      <!-- Ajuste '5rem' conforme a altura do header -->
      <div class="max-w-xl">
        <h1 class="text-4xl md:text-4xl lg:text-5xl font-bold text-white leading-tight">
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
