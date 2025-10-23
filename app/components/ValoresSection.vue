<template>
  <section id="valores" class="py-20 bg-gray-50 overflow-hidden">
    <div class="max-w-7xl mx-auto px-6">
      <h2 class="text-3xl font-bold text-center mb-16 text-primary-400">
        Nossos Valores
      </h2>

      <div class="flex flex-col gap-8">
        <!-- Card 1 -->
        <div class="card-valor flex justify-start opacity-0 translate-y-10 transition-all duration-700 ease-out">
          <div class="flex flex-col sm:flex-row items-center gap-4 sm:gap-6 bg-white rounded-xl shadow-md hover:shadow-xl transition-all duration-300 hover:scale-[1.02] w-full sm:max-w-3xl md:h-28 px-6 sm:px-8 py-6">
            <img src="" alt="Inovação" class="w-14 h-14" />
            <div class="text-center sm:text-left">
              <h3 class="text-xl font-semibold text-primary-400">Inovação</h3>
              <p class="text-gray-600 text-sm mt-1">
                Buscamos soluções criativas e eficientes em cada projeto.
              </p>
            </div>
          </div>
        </div>

        <!-- Card 2 -->
        <div class="card-valor flex justify-end opacity-0 translate-y-10 transition-all duration-700 ease-out">
          <div class="flex flex-col sm:flex-row-reverse items-center gap-4 sm:gap-6 bg-white rounded-xl shadow-md hover:shadow-xl transition-all duration-300 hover:scale-[1.02] w-full sm:max-w-3xl md:h-28 px-6 sm:px-8 py-6">
            <img src="" alt="Compromisso" class="w-14 h-14" />
            <div class="text-center sm:text-right">
              <h3 class="text-xl font-semibold text-primary-400">Compromisso</h3>
              <p class="text-gray-600 text-sm mt-1">
                Nos dedicamos a entregar excelência e responsabilidade.
              </p>
            </div>
          </div>
        </div>

        <!-- Card 3 -->
        <div class="card-valor flex justify-start opacity-0 translate-y-10 transition-all duration-700 ease-out">
          <div class="flex flex-col sm:flex-row items-center gap-4 sm:gap-6 bg-white rounded-xl shadow-md hover:shadow-xl transition-all duration-300 hover:scale-[1.02] w-full sm:max-w-3xl md:h-28 px-6 sm:px-8 py-6">
            <img src="" alt="Qualidade" class="w-14 h-14" />
            <div class="text-center sm:text-left">
              <h3 class="text-xl font-semibold text-primary-400">Qualidade</h3>
              <p class="text-gray-600 text-sm mt-1">
                Garantimos alto padrão em todas as etapas do processo.
              </p>
            </div>
          </div>
        </div>

        <!-- Card 4 -->
        <div class="card-valor flex justify-end opacity-0 translate-y-10 transition-all duration-700 ease-out">
          <div class="flex flex-col sm:flex-row-reverse items-center gap-4 sm:gap-6 bg-white rounded-xl shadow-md hover:shadow-xl transition-all duration-300 hover:scale-[1.02] w-full sm:max-w-3xl md:h-28 px-6 sm:px-8 py-6">
            <img src="" alt="Transparência" class="w-14 h-14" />
            <div class="text-center sm:text-right">
              <h3 class="text-xl font-semibold text-primary-400">Transparência</h3>
              <p class="text-gray-600 text-sm mt-1">
                Prezamos pela clareza e confiança nas relações com clientes.
              </p>
            </div>
          </div>
        </div>

        <!-- Card 5 -->
        <div class="card-valor flex justify-start opacity-0 translate-y-10 transition-all duration-700 ease-out">
          <div class="flex flex-col sm:flex-row items-center gap-4 sm:gap-6 bg-white rounded-xl shadow-md hover:shadow-xl transition-all duration-300 hover:scale-[1.02] w-full sm:max-w-3xl md:h-28 px-6 sm:px-8 py-6">
            <img src="" alt="Sustentabilidade" class="w-14 h-14" />
            <div class="text-center sm:text-left">
              <h3 class="text-xl font-semibold text-primary-400">Sustentabilidade</h3>
              <p class="text-gray-600 text-sm mt-1">
                Promovemos práticas conscientes e respeito ao meio ambiente.
              </p>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>
</template>

<script setup>
import { onMounted } from 'vue'

onMounted(() => {
  const cards = document.querySelectorAll('.card-valor')

  const observer = new IntersectionObserver(
    (entries, observer) => {
      entries.forEach((entry, index) => {
        if (entry.isIntersecting) {
          setTimeout(() => {
            entry.target.classList.remove('opacity-0', 'translate-y-10')
            entry.target.classList.add('opacity-100', 'translate-y-0')
          }, index * 200) // delay escalonado
          observer.unobserve(entry.target)
        }
      })
    },
    { threshold: 0.2 }
  )

  cards.forEach((card) => observer.observe(card))
})
</script>
