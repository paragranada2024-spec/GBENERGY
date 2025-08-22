<template>
  <div class="relative bg-gradient-to-br from-blue-50  to-gray-50  ">
  <section 
    id="accueil" 
    class=" flex items-center justify-center px-4 sm:px-6 lg:px-8 py-10 "
  >
    <div class="max-w-4xl text-center ">
      <h1 class="text-xl lg:text-3xl font-bold text-gray-900 my-8  leading-tight">
        Votre partenaire en 
        <span class="text-blue-600">énergie électrique</span>
        au Maroc
      </h1>
      <p class="text-lg lg:text-xl text-gray-600 mb-8 leading-relaxed">
        GB ENERGY vous accompagne dans tous vos projets d'installations électriques, 
        pneumatiques et photovoltaïques avec expertise et professionnalisme.
      </p>
      <div class="flex flex-col sm:flex-row gap-4 justify-center">
        <a href="#contact" class="bg-blue-600 text-white px-8 py-4 rounded-lg text-lg font-semibold hover:bg-blue-700 transition-all duration-300 shadow-lg hover:shadow-xl">
          Demander un devis gratuit
        </a>
        <a href="#services" class="border-2 border-blue-600 text-blue-600 px-8 py-4 rounded-lg text-lg font-semibold hover:bg-blue-50 transition-all duration-300">
          Nos services
        </a>
      </div>
    </div>
  </section>
  <section id="a-propos" class="pt-20 pb-4 my-10 mb-0 ">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-3xl lg:text-4xl font-bold text-gray-900 mb-4">
          Pourquoi choisir GB ENERGY ?
        </h2>
        <p class="text-xl text-gray-600 max-w-3xl mx-auto">
          Avec plus de 10 ans d'expérience, nous sommes votre partenaire de confiance 
          pour tous vos projets énergétiques au Maroc.
        </p>
      </div>
      
      <!-- <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
        <div v-for="feature in features" :key="feature.title" class="text-center group">
          <div class="bg-blue-50 rounded-full w-16 h-16 flex items-center justify-center mx-auto mb-4 group-hover:bg-blue-200 transition-colors">
            <component :is="feature.icon" class="w-8 h-8 text-blue-600" />
          </div>
          <h3 class="text-xl font-semibold text-gray-900 mb-2">{{ feature.title }}</h3>
          <p class="text-gray-600">{{ feature.description }}</p>
        </div>
      </div> -->
    </div>
  </section>
  </div>
</template>

<script setup>

</script>