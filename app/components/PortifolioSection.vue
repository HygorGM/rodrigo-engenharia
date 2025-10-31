<template>
  <section
    id="portifolio"
    class="w-full py-16 bg-gray-100"
    aria-label="Portfólio de clientes e parceiros"
  >
    <div class="text-center mb-10">
      <h2 class="text-3xl md:text-4xl font-bold text-gray-800">
        Portfólio
      </h2>
      <div class="w-24 h-[3px] bg-orange-500 mx-auto mt-3 rounded-full" />
      <p class="text-gray-600 mt-4 max-w-xl mx-auto">
        Algumas empresas e parceiros que confiam em nossos serviços de engenharia civil.
      </p>
    </div>

    <div
      class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 gap-6 px-6 md:px-20"
    >
      <div
        class="flex items-center justify-center bg-white p-4 rounded-xl shadow-md hover:shadow-xl transition-transform transform hover:-translate-y-2 duration-300"
      >
        <img
          src="/imagens/academia-fitmusic.png"
          alt="Logo empresa 1"
          class="object-contain max-h-16"
        >
      </div>

      <div
        class="flex items-center justify-center bg-white p-4 rounded-xl shadow-md hover:shadow-xl transition-transform transform hover:-translate-y-2 duration-300"
      >
        <img
          src="/imagens/ad-campinas.png"
          alt="Logo empresa 2"
          class="object-contain max-h-16"
        >
      </div>

      <div
        class="flex items-center justify-center bg-white p-4 rounded-xl shadow-md hover:shadow-xl transition-transform transform hover:-translate-y-2 duration-300"
      >
        <img
          src="/imagens/casas-mh.png"
          alt="Logo empresa 3"
          class="object-contain max-h-16"
        >
      </div>

      <div
        class="flex items-center justify-center bg-white p-4 rounded-xl shadow-md hover:shadow-xl transition-transform transform hover:-translate-y-2 duration-300"
      >
        <img
          src="/imagens/correios.png"
          alt="Logo empresa 4"
          class="object-contain max-h-16"
        >
      </div>

      <div
        class="flex items-center justify-center bg-white p-4 rounded-xl shadow-md hover:shadow-xl transition-transform transform hover:-translate-y-2 duration-300"
      >
        <img
          src="/imagens/imper-laje.png"
          alt="Logo empresa 5"
          class="object-contain max-h-16"
        >
      </div>

      <div
        class="flex items-center justify-center bg-white p-4 rounded-xl shadow-md hover:shadow-xl transition-transform transform hover:-translate-y-2 duration-300"
      >
        <img
          src="/imagens/impertudo.png"
          alt="Logo empresa 6"
          class="object-contain max-h-16"
        >
      </div>

      <div
        class="flex items-center justify-center bg-white p-4 rounded-xl shadow-md hover:shadow-xl transition-transform transform hover:-translate-y-2 duration-300"
      >
        <img
          src="/imagens/jn&j.png"
          alt="Logo empresa 7"
          class="object-contain max-h-16"
        >
      </div>

      <div
        class="flex items-center justify-center bg-white p-4 rounded-xl shadow-md hover:shadow-xl transition-transform transform hover:-translate-y-2 duration-300"
      >
        <img
          src="/imagens/mjc.png"
          alt="Logo empresa 8"
          class="object-contain max-h-16"
        >
      </div>

      <div
        class="flex items-center justify-center bg-white p-4 rounded-xl shadow-md hover:shadow-xl transition-transform transform hover:-translate-y-2 duration-300"
      >
        <img
          src="/imagens/pormade-portas.png"
          alt="Logo empresa 9"
          class="object-contain max-h-16"
        >
      </div>

      <div
        class="flex items-center justify-center bg-white p-4 rounded-xl shadow-md hover:shadow-xl transition-transform transform hover:-translate-y-2 duration-300"
      >
        <img
          src="/imagens/rezende-arantes.png"
          alt="Logo empresa 10"
          class="object-contain max-h-16"
        >
      </div>

      <div
        class="flex items-center justify-center bg-white p-4 rounded-xl shadow-md hover:shadow-xl transition-transform transform hover:-translate-y-2 duration-300"
      >
        <img
          src="/imagens/terral-incorporadora.png"
          alt="Logo empresa 11"
          class="object-contain max-h-16"
        >
      </div>
    </div>
  </section>
</template>

<style scoped>
section {
  scroll-margin-top: 80px; /* caso o header seja fixo */
}
</style>
