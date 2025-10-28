<template>
  <section
    id="contatos"
    class="w-full py-16 "
    aria-label="Entre em contato"
  >
    <div class="text-center mb-10">
      <h2 class="text-3xl md:text-4xl font-bold text-gray-800">
        Contatos
      </h2>
      <div class="w-24 h-[3px] bg-orange-500 mx-auto mt-3 rounded-full" />
    </div>

    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6 max-w-5xl mx-auto px-6">
      <a
        href="https://www.instagram.com/engrodrigomr/"
        target="_blank"
        class="flex flex-col items-center bg-gray-50 p-6 rounded-2xl shadow-sm hover:shadow-lg hover:-translate-y-1 transform transition duration-300 border border-transparent hover:border-orange-200 group"
      >
        <div
          class="w-16 h-16 flex items-center justify-center rounded-full mb-3 relative icon-circle"
        >
          <div class="absolute inset-0 rounded-full gradient-bg" />
          <img
            src="/imagens/Instagram.png"
            alt="Ícone do Instagram"
            class="w-8 h-8 object-contain relative z-10"
          >
        </div>
        <h3 class="text-base font-semibold text-gray-800 group-hover:text-orange-600 transition">
          Instagram
        </h3>
        <p class="text-gray-600 mt-1 text-sm">engrodrigomr</p>
      </a>

      <a
        href="https://wa.me/message/MJHWYM756SHTA1"
        target="_blank"
        class="flex flex-col items-center bg-gray-50 p-6 rounded-2xl shadow-sm hover:shadow-lg hover:-translate-y-1 transform transition duration-300 border border-transparent hover:border-green-200 group"
      >
        <div
          class="w-16 h-16 flex items-center justify-center rounded-full mb-3 relative icon-circle"
          style="background: transparent;"
        >
          <div class="absolute inset-0 rounded-full gradient-green" />
          <img
            src="/imagens/whatsapp.png"
            alt="Ícone do WhatsApp"
            class="w-8 h-8 object-contain relative z-10"
          >
        </div>
        <h3 class="text-base font-semibold text-gray-800 group-hover:text-green-600 transition">
          WhatsApp
        </h3>
        <p class="text-gray-600 mt-1 text-sm">(62) 99394-2206</p>
      </a>

      <a
        href="https://mail.google.com/mail/?view=cm&fs=1&to=engrodrigomarquesr@gmail.com"
        target="_blank"
        rel="noopener noreferrer"
        class="flex flex-col items-center bg-gray-50 p-6 rounded-2xl shadow-sm hover:shadow-lg hover:-translate-y-1 transform transition duration-300 border border-transparent hover:border-red-200 group"
      >
        <div
          class="w-16 h-16 flex items-center justify-center rounded-full mb-3 relative icon-circle"
          style="background: transparent;"
        >
          <div class="absolute inset-0 rounded-full gradient-red" />
          <img
            src="/imagens/gmail.png"
            alt="Ícone do e-mail"
            class="w-8 h-8 object-contain relative z-10"
          >
        </div>
        <h3 class="text-base font-semibold text-gray-800 group-hover:text-red-600 transition">
          E-mail
        </h3>
        <p class="text-gray-600 mt-1 text-sm">engrodrigomarquesr@gmail.com</p>
      </a>
    </div>
  </section>
</template>

<style scoped>
section { scroll-margin-top: 80px; }

.icon-circle {
  will-change: transform, opacity;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  overflow: visible;
  transition: transform 300ms ease;
  animation: pulse-slow 3.2s infinite ease-in-out;
}

.gradient-bg {
  background: linear-gradient(45deg, #feda75 0%, #f58529 30%, #dd2a7b 60%, #8134af 100%);
  z-index: 0;
  opacity: 0.9;
}

.gradient-green {
  background: linear-gradient(180deg, #34d399 0%, #10b981 100%);
  z-index: 0;
  opacity: 0.9;
}

.gradient-red {
  background: linear-gradient(180deg, #fb7185 0%, #f43f5e 100%);
  z-index: 0;
  opacity: 0.9;
}

.icon-circle img {
  z-index: 10;
  position: relative;
}

.group:hover .icon-circle {
  transform: scale(1.08);
  animation-duration: 1.2s;
}

@keyframes pulse-slow {
  0%   { transform: scale(1); opacity: 0.88; }
  50%  { transform: scale(1.06); opacity: 1; }
  100% { transform: scale(1); opacity: 0.88; }
}
</style>
