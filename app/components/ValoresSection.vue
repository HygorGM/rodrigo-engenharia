<template>
  <section class="flex flex-col w-full">
    <div class="text-center my-8">
      <h2 class="text-2xl md:text-3xl font-bold text-gray-800">
        Nossos Valores
      </h2>
      <div class="w-20 h-[3px] bg-orange-500 mx-auto mt-2 rounded-full"></div>
    </div>

    <div class="flex flex-col">
      <!-- Card 1 -->
      <div
        class="relative group min-h-[180px] md:min-h-[220px] lg:min-h-[260px] flex items-center text-white overflow-hidden cursor-pointer transition-all duration-500"
      >
        <img
          src="/imagens/Engenheiro analise de obra.jpeg"
          alt="Excelência"
          class="absolute inset-0 w-full h-full object-cover transition-all duration-500 group-hover:brightness-75 bg-gray-800/50"
        />
        <div
          class="absolute inset-0 bg-black/40 group-hover:bg-black/60 transition-all duration-500"
        ></div>
        <div class="relative z-10 w-full max-w-7xl mx-auto px-8 md:px-10 lg:px-16">
          <h3 class="text-lg md:text-xl font-bold mb-1">Excelência</h3>
          <p class="text-sm md:text-base max-w-[700px] leading-snug">
            Comprometidos em entregar soluções de engenharia civil com o mais alto padrão de qualidade, buscando precisão em cada etapa, desde o planejamento até a execução, para garantir obras seguras, duráveis e eficientes.

          </p>
        </div>
      </div>

      <!-- Card 2 -->
      <div
        class="relative group min-h-[180px] md:min-h-[220px] lg:min-h-[260px] flex items-center text-white overflow-hidden cursor-pointer transition-all duration-500"
      >
        <img
          src="/imagens/Nivel para medir.png"
          alt="Manutenção e Higienização"
          class="absolute inset-0 w-full h-full object-cover transition-all duration-500 group-hover:brightness-75 bg-gray-800/50"
        />
        <div
          class="absolute inset-0 bg-black/40 group-hover:bg-black/60 transition-all duration-500"
        ></div>
        <div class="relative z-10 w-full max-w-7xl mx-auto px-8 md:px-10 lg:px-16">
          <h3 class="text-lg md:text-xl font-bold mb-1">
            Inovação
          </h3>
          <p class="text-sm md:text-base max-w-[700px] leading-snug">
            Aplicamos tecnologias avançadas e métodos modernos para desenvolver soluções de engenharia mais precisas, sustentáveis e eficientes.
          </p>
        </div>
      </div>

      <!-- Card 3 -->
      <div
        class="relative group min-h-[180px] md:min-h-[220px] lg:min-h-[260px] flex items-center text-white overflow-hidden cursor-pointer transition-all duration-500"
      >
        <img
          src="/imagens/Contador.jpeg"
          alt="Pré-instalação"
          class="absolute inset-0 w-full h-full object-cover transition-all duration-500 group-hover:brightness-75 bg-gray-800/50"
        />
        <div
          class="absolute inset-0 bg-black/40 group-hover:bg-black/60 transition-all duration-500"
        ></div>
        <div class="relative z-10 w-full max-w-7xl mx-auto px-8 md:px-10 lg:px-16">
          <h3 class="text-lg md:text-xl font-bold mb-1">Compromisso</h3>
          <p class="text-sm md:text-base max-w-[700px] leading-snug">
           Respeito aos prazos, orçamentos e
           expectativas dos clientes.

 
          </p>
        </div>
      </div>

      <!-- Card 4 -->
      
      <div
        class="relative group min-h-[180px] md:min-h-[220px] lg:min-h-[260px] flex items-center text-white overflow-hidden cursor-pointer transition-all duration-500"
      >
        <img
          src="/imagens/Engenheiro-visitando-obra.jpeg"
          alt="Consultoria Técnica"
          class="absolute inset-0 w-full h-full object-cover transition-all duration-500 group-hover:brightness-75 bg-gray-800/50"
        />
        <div
          class="absolute inset-0 bg-black/40 group-hover:bg-black/60 transition-all duration-500"
        ></div>
        <div class="relative z-10 w-full max-w-7xl mx-auto px-8 md:px-10 lg:px-16">
          <h3 class="text-lg md:text-xl font-bold mb-1">Sofisticação</h3>
          <p class="text-sm md:text-base max-w-[700px] leading-snug">
            Atenção aos mínimos detalhes
            para garantir alto padrão nos
            acabamentos.

          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
// Apenas efeitos visuais
</script>

<style scoped>
.group:hover img {
  transform: scale(1.05);
}
</style>
