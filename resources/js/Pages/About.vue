<template>

  <div class="min-h-screen bg-gray-50">
    <AppHeader />
    <!-- Header Section -->
    <section class="bg-blue-600 text-white py-16">
      <div class="max-w-4xl mx-auto px-6 text-center">
        <h1 class="text-4xl md:text-5xl font-bold mb-4">À propos de GB ENERGY</h1>
        <p class="text-xl md:text-2xl text-blue-100">
          Votre partenaire de confiance pour tous vos besoins énergétiques
        </p>
      </div>
    </section>

    <!-- Main Content -->
    <main class="max-w-6xl mx-auto px-6 py-16 space-y-20">
      <HistorySections />
      <ValuesSections />
      <VisionSections />
    </main>

    <!-- Call to Action Section -->
    <section class="bg-blue-600 text-white py-16">
      <div class="max-w-4xl mx-auto px-6 text-center">
        <h2 class="text-3xl font-bold mb-4">Prêt à travailler avec nous ?</h2>
        <p class="text-xl text-blue-100 mb-8">Contactez-nous dès aujourd'hui pour discuter de votre projet</p>
        <button class="bg-white text-blue-600 px-8 py-3 rounded-lg font-semibold hover:bg-gray-100 transition-colors">
          Nous contacter
        </button>
      </div>
    </section>
    <AppFooter />
  </div>
</template>

<script setup>
import { onMounted } from 'vue'
import HistorySections from '@/Components/About/HistorySections.vue'
import ValuesSections from '@/Components/About/ValuesSections.vue'
import VisionSections from '@/Components/About/VisionSections.vue'
import DefaultLayout from '@/Layouts/DefaultLayout.vue'

onMounted(() => {
  document.title = 'À propos - GB ENERGY'
  
  // Update meta description
  let metaDescription = document.querySelector('meta[name="description"]')
  if (!metaDescription) {
    metaDescription = document.createElement('meta')
    metaDescription.name = 'description'
    document.head.appendChild(metaDescription)
  }
  metaDescription.content = 'Découvrez l\'histoire, les valeurs et la vision de GB ENERGY, votre partenaire de confiance depuis 2018.'
})

defineOptions({
  layout:DefaultLayout
})
</script>
