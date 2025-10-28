<template>
  <footer class="bg-gray-900 text-gray-300 py-10">
    <div
      class="max-w-7xl mx-auto px-6 grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-8"
    >
      <div class="flex flex-col items-start">
        <div class="flex items-center space-x-2 mb-4">
          <h3 class="text-xl font-bold text-white">
            RM Engenharia
          </h3>
        </div>
        <p class="text-sm text-gray-400 leading-relaxed">
          Soluções modernas e eficientes em engenharia civil, unindo tecnologia
          e qualidade em cada projeto.
        </p>
      </div>

      <div>
        <h4 class="text-lg font-semibold text-white mb-3">
          Navegação
        </h4>
        <ul class="space-y-2">
          <li>
            <a
              href="#inicio"
              class="hover:text-orange-500"
            >Início</a>
          </li>
          <li>
            <a
              href="#sobre"
              class="hover:text-orange-500"
            >Sobre</a>
          </li>
          <li>
            <a
              href="#servicos"
              class="hover:text-orange-500"
            >Serviços</a>
          </li>
          <li>
            <a
              href="#portifolio"
              class="hover:text-orange-500"
            >Portfólio</a>
          </li>
          <li>
            <a
              href="#contatos"
              class="hover:text-orange-500"
            >Contatos</a>
          </li>
        </ul>
      </div>

      <div>
        <h4 class="text-lg font-semibold text-white mb-3">
          Contato
        </h4>
        <ul class="space-y-2 text-sm">
          <li>
            <a
              href="https://mail.google.com/mail/?view=cm&fs=1&to=engrodrigomarquesr@gmail.com"
              target="_blank"
              rel="noopener noreferrer"
              class="flex items-center gap-2 hover:text-orange-500 transition"
            >
              <i class="fa-solid fa-envelope text-orange-500" />
              <span class="break-words max-w-full">engrodrigomarquesr@gmail.com</span>
            </a>
          </li>
          <li>
            <a
              href="https://wa.me/message/MJHWYM756SHTA1"
              target="_blank"
              rel="noopener noreferrer"
              class="flex items-center gap-2 hover:text-orange-500 transition"
            >
              <i class="fa-brands fa-whatsapp text-green-500" />
              <span>(62) 99394-2206</span>
            </a>
          </li>
          <li>
            <a
              href="https://www.instagram.com/engrodrigomr/"
              target="_blank"
              rel="noopener noreferrer"
              class="flex items-center gap-2 hover:text-orange-500 transition"
            >
              <i class="fa-brands fa-instagram text-pink-500" />
              <span>engrodrigomr</span>
            </a>
          </li>
        </ul>
      </div>

      <div>
        <h4 class="text-lg font-semibold text-white mb-3">
          Localização
        </h4>
        <p class="text-sm text-gray-400 leading-relaxed">
          Rua Exemplo, 123 <br>
          Bairro Central <br>
          Cidade - UF
        </p>
      </div>
    </div>

    <div class="border-t border-gray-700 mt-10 pt-6 text-center text-sm text-gray-400">
      <p>
        © {{ new Date().getFullYear() }} RM Engenharia — Todos os direitos
        reservados.
      </p>
      <p class="mt-1">
        Desenvolvido por <span class="text-orange-500 font-semibold">HygorGM</span>
      </p>
    </div>
  </footer>
</template>

<style scoped>
footer {
  scroll-margin-top: 80px;
}
</style>
