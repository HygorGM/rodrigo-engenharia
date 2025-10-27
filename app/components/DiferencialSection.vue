<template>
  <section id="diferenciais" class="py-20 bg-gray-50">
    <div class="max-w-7xl mx-auto px-6">
      <div class="grid grid-cols-1 lg:grid-cols-2 items-center gap-12">

        <!-- imagem -->
        <div class="order-1 lg:order-1 relative">
          <img 
            src="/imagens/Edificio 1.jpeg" 
            alt="Diferenciais" 
            class="w-full h-auto rounded-xl shadow-xl transition-transform duration-500 hover:scale-105" 
          /> 
          <div class="hidden lg:block absolute top-0 right-[-24px] h-full w-[4px] bg-orange-500 rounded-full"></div>
        </div>

        <!-- Cards -->
        <div class="order-2 lg:order-2 flex flex-col gap-6">
          <h2 class="text-3xl font-bold text-primary-400 mb-4">
            Nossos <span class="text-primary-400">Diferenciais</span>
          </h2>

          <div class="flex flex-col gap-4">
            <div class="bg-orange-400 text-white rounded-xl p-6 shadow-md transform transition-all duration-500 hover:shadow-2xl hover:-translate-y-2 hover:bg-orange-500">
              <h3 class="font-semibold text-lg mb-2">Atendimento Consultivo e Relacionamento Diferenciado</h3>
              <p class="text-sm">
                Acompanhamento próximo e transparente do cliente, com comunicação eficiente e suporte técnico especializado em todas as fases da obra.
              </p>
            </div>

            <div class="bg-orange-400 text-white rounded-xl p-6 shadow-md transform transition-all duration-500 hover:shadow-2xl hover:-translate-y-2 hover:bg-orange-500">
              <h3 class="font-semibold text-lg mb-2">Especialização em Obras de Alto Padrão</h3>
              <p class="text-sm">
                Experiência e know-how na construção e reforma de residências e empreendimentos comerciais sofisticados, garantindo acabamentos impecáveis e atenção aos mínimos detalhes.
              </p>
            </div>

            <div class="bg-orange-400 text-white rounded-xl p-6 shadow-md transform transition-all duration-500 hover:shadow-2xl hover:-translate-y-2 hover:bg-orange-500">
              <h3 class="font-semibold text-lg mb-2">Gerenciamento Estratégico e Cumprimento de Prazos</h3>
              <p class="text-sm">
                Execução eficiente e planejada, garantindo o controle total de custos e prazos, sem comprometer a qualidade.
              </p>
            </div>
          </div>

          <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mt-6">
            <div class="bg-orange-500 rounded-xl text-center p-4 shadow-md transform transition-transform duration-300 hover:scale-105">
              <p class="text-2xl font-bold">+10.000m²</p>
              <p class="text-sm">Construídos</p>
            </div>
            <div class="bg-orange-500 rounded-xl text-center p-4 shadow-md transform transition-transform duration-300 hover:scale-105">
              <p class="text-2xl font-bold">+40</p>
              <p class="text-sm">Clientes atendidos em 2024</p>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>
</template>
