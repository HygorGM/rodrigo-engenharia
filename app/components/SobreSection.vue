<template>
  <section
    id="sobre"
    class="w-full py-16 bg-white dark:bg-gray-900 overflow-hidden"
    role="region"
    aria-label="Seção sobre a empresa"
  >
    <div class="max-w-7xl mx-auto px-6 md:px-10 lg:px-16 grid md:grid-cols-2 gap-10 items-center">
      <div>
        <h2 class="text-4xl md:text-5xl font-extrabold mb-6">
          <span class="text-gray-900 dark:text-white">Quem</span>
          <span class="text-orange-500"> Somos?</span>
        </h2>

        <p class="text-gray-700 dark:text-gray-300 mb-4">
          A <strong>RM Engenharia</strong> nasceu com um propósito claro: oferecer
          serviços de execução de obras, reformas e soluções técnicas
          <strong>em alto padrão, com qualidade superior, sofisticação e uso de tecnologias inovadoras.</strong>
        </p>

        <p class="text-gray-700 dark:text-gray-300 mb-4">
          Prezamos por ser uma <strong>referência no ramo da construção civil</strong>,
          combinando <strong>atendimento personalizado</strong>, inovação e
          comprometimento com prazos e orçamentos.
        </p>

        <p class="text-gray-700 dark:text-gray-300">
          Nossa equipe é formada por profissionais com vasta experiência no setor,
          garantindo um alto nível técnico em cada serviço realizado.
        </p>

        <p class="mt-6 text-gray-700 dark:text-gray-300">
          Com atuação em <strong>Goiânia e região</strong>, a RM Engenharia vem se consolidando
          como um nome de confiança para aqueles que buscam excelência em cada detalhe.
        </p>
      </div>

      <!-- Imagem  -->
      <div class="flex justify-center md:justify-end">
        <div class="relative group rounded-lg overflow-hidden shadow-lg max-w-md transition-transform duration-300">
          <img
            src="/imagens/engenheiro trabalhando.jpeg"
            alt="Engenheiro civil trabalhando em obra"
            class="w-full h-auto object-cover transform group-hover:scale-105 transition-transform duration-500 ease-in-out"
            loading="lazy"
          />

          <div
            class="absolute inset-0 bg-orange-500/0 group-hover:bg-orange-500/20 transition-colors duration-500 ease-in-out"
          ></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
@media (max-width: 768px) {
  h2 {
    text-align: center;
  }
}
</style>