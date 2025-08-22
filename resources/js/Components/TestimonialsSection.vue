<template>
  <section class="py-20 bg-gradient-to-br from-blue-50 to-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-3xl lg:text-4xl font-bold text-gray-900 mb-4">
          Ils nous font confiance
        </h2>
        <p class="text-xl text-gray-600">
          Découvrez les témoignages de nos clients satisfaits
        </p>
      </div>
      
      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        <div v-for="testimonial in testimonials" :key="testimonial.name" 
             class="bg-white rounded-xl p-6 shadow-lg">
          <div class="flex items-center mb-4">
            <div v-for="i in 5" :key="i" class="text-yellow-400">
              <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20">
                <path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z" />
              </svg>
            </div>
          </div>
          <p class="text-gray-600 mb-4 italic">"{{ testimonial.comment }}"</p>
          <div class="flex items-center">
            <div class="w-10 h-10 bg-blue-100 rounded-full flex items-center justify-center mr-3">
              <span class="text-blue-600 font-semibold">{{ testimonial.name.charAt(0) }}</span>
            </div>
            <div>
              <p class="font-semibold text-gray-900">{{ testimonial.name }}</p>
              <p class="text-sm text-gray-600">{{ testimonial.company }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const testimonials = [
  {
    name: "Ahmed Benali",
    company: "Restaurant Le Palmier",
    comment: "Installation électrique parfaite pour notre restaurant. Équipe professionnelle et délais respectés."
  },
  {
    name: "Fatima Alaoui",
    company: "Usine Textile Casablanca",
    comment: "GB ENERGY a modernisé toute notre installation industrielle. Excellent travail et suivi impeccable."
  },
  {
    name: "Mohamed Tazi",
    company: "Villa privée Rabat",
    comment: "Panneaux solaires installés rapidement. Économies d'énergie visibles dès le premier mois."
  }
]
</script>