<template>
  <div class="min-h-screen bg-gray-50">
    <!-- Header -->
    <Header />

    <!-- Hero Section -->
    <section class="bg-gradient-to-r from-blue-600 to-blue-700 text-white py-16">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h1 class="text-4xl md:text-5xl font-bold mb-6">Nos Services</h1>
        <p class="text-xl text-blue-100 max-w-3xl mx-auto">
          Des solutions complètes en électricité, pneumatique et photovoltaïque pour les secteurs tertiaire et
          industriel au Maroc
        </p>
      </div>
    </section>

    <!-- Services Grid -->
    <section class="py-16">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 md:grid-cols-4 gap-3 ">

          <!-- Secteur Tertiaire -->
          <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
            <img src="/src/assets/Tertaire.jpg" alt="Tertaire" class="w-full h-40 object-cover rounded-t-2xl" />
            <div class="p-8 pt-5">
              <div class="flex items-center mb-6">
                <h2 class="text-2xl font-bold text-blue-950">Secteur Tertiaire</h2>
              </div>

              <div class="grid  gap-6 mb-8">
                <div class="space-y-4">
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">Installations Électriques</h3>
                      <p class="text-gray-600">Conception et réalisation d'installations électriques complètes</p>
                    </div>
                  </div>
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">Domotique</h3>
                      <p class="text-gray-600">Solutions intelligentes pour l'automatisation des bâtiments</p>
                    </div>
                  </div>
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">Câblage</h3>
                      <p class="text-gray-600">Réseaux de câblage structuré et distribution électrique</p>
                    </div>
                  </div>
                </div>
                <div class="space-y-4">
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">Vidéosurveillance</h3>
                      <p class="text-gray-600">Systèmes de sécurité et surveillance vidéo</p>
                    </div>
                  </div>
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">Systèmes d'Alarme</h3>
                      <p class="text-gray-600">Protection et sécurisation des locaux</p>
                    </div>
                  </div>
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">Maintenance</h3>
                      <p class="text-gray-600">Entretien préventif et curatif des installations</p>
                    </div>
                  </div>
                </div>
              </div>

              <div class="flex flex-col sm:flex-row gap-4">
                <button @click="requestQuote('Secteur Tertiaire')"
                  class="bg-blue-600 text-white px-8 py-3 mt-[7.2rem] rounded-lg hover:bg-blue-700 transition-colors font-medium">
                  Demander un devis
                </button>

              </div>
            </div>
          </div>

          <!-- Secteur Industriel -->
          <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
            <img src="/src/assets/Industrielle.jpg" alt="Industrielle" class="w-full h-40 object-cover rounded-t-2xl" />
            <div class="p-8 pt-5">
              <div class="flex items-center mb-6">
                <h2 class="text-2xl font-bold text-blue-950">Secteur Industriel</h2>
              </div>

              <div class="grid  gap-6 mb-8">
                <div class="space-y-4">
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">Réseaux Électriques</h3>
                      <p class="text-gray-600">Installation et maintenance de réseaux électriques industriels</p>
                    </div>
                  </div>
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">Réseaux Pneumatiques</h3>
                      <p class="text-gray-600">Systèmes d'air comprimé et automatisation pneumatique</p>
                    </div>
                  </div>
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">Armoires Électriques</h3>
                      <p class="text-gray-600">Conception et assemblage d'armoires de commande</p>
                    </div>
                  </div>
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">Moteurs</h3>
                      <p class="text-gray-600">Installation et maintenance de moteurs industriels</p>
                    </div>
                  </div>
                </div>
                <div class="space-y-4">
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">Groupes Électrogènes</h3>
                      <p class="text-gray-600">Solutions d'alimentation de secours et continue</p>
                    </div>
                  </div>
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">HTA (Haute Tension)</h3>
                      <p class="text-gray-600">Installations haute tension et postes de transformation</p>
                    </div>
                  </div>
                  <div class="flex items-start space-x-3">

                    <div>
                      <h3 class="font-semibold text-gray-900">Sécurité Incendie</h3>
                      <p class="text-gray-600">Systèmes de détection et protection incendie</p>
                    </div>
                  </div>
                </div>
              </div>

              <div class="flex flex-col sm:flex-row gap-4">
                <button @click="requestQuote('Secteur Industriel')"
                  class="bg-gray-600 text-white px-8 py-3 mt-[3.3rem] rounded-lg hover:bg-gray-700 transition-colors font-medium">
                  Demander un devis
                </button>

              </div>
            </div>
          </div>

          <!-- Photovoltaïque -->
          <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
            <img src="/src/assets/Photovoltaïque.jpg" alt="Photovoltaïque"
              class="w-full h-40 object-cover rounded-t-2xl" />
            <div class="p-8 pt-5">
              <div class="flex items-center mb-6">
                <h2 class="text-2xl font-bold text-blue-950">Photovoltaïque & Énergie Renouvelable</h2>
              </div>
              <div class="mb-8">
                <Swiper :modules="modules" :slides-per-view="1" :space-between="20" :loop="true"
                  :autoplay="{ delay: 4000, disableOnInteraction: false }" :pagination="{ clickable: true }"
                  class="w-full">
                  <!-- Slide 1 -->
                  <SwiperSlide class=" mb-7">
                    <div class="text-center ">
                      <div class="w-12 h-12 bg-yellow-100 rounded-lg flex items-center justify-center mx-auto mb-4">
                        <svg class="w-6 h-6 text-yellow-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z" />
                        </svg>
                      </div>
                      <h3 class="font-semibold text-gray-900 mb-2">Étude</h3>
                      <p class="text-gray-600">
                        Analyse de faisabilité et dimensionnement des installations solaires
                      </p>
                    </div>
                  </SwiperSlide>

                  <!-- Slide 2 -->
                  <SwiperSlide>
                    <div class="text-center">
                      <div class="w-12 h-12 bg-yellow-100 rounded-lg flex items-center justify-center mx-auto mb-4">
                        <svg class="w-6 h-6 text-yellow-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M19.428 15.428a2 2 0 00-1.022-.547l-2.387-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547M8 4h8l-1 1v5.172a2 2 0 00.586 1.414l5 5c1.26 1.26.367 3.414-1.415 3.414H4.828c-1.782 0-2.674-2.154-1.414-3.414l5-5A2 2 0 009 10.172V5L8 4z" />
                        </svg>
                      </div>
                      <h3 class="font-semibold text-gray-900 mb-2">Installation</h3>
                      <p class="text-gray-600">
                        Pose et raccordement de panneaux solaires et onduleurs
                      </p>
                    </div>
                  </SwiperSlide>

                  <!-- Slide 3 -->
                  <SwiperSlide>
                    <div class="text-center">
                      <div class="w-12 h-12 bg-yellow-100 rounded-lg flex items-center justify-center mx-auto mb-4">
                        <svg class="w-6 h-6 text-yellow-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z" />
                          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                        </svg>
                      </div>
                      <h3 class="font-semibold text-gray-900 mb-2">Maintenance</h3>
                      <p class="text-gray-600">
                        Suivi des performances et maintenance préventive
                      </p>
                    </div>
                  </SwiperSlide>
                </Swiper>

                <!-- Pagination dots (Swiper adds them here) -->
                <div class="swiper-pagination mt-6"></div>
              </div>

              <div class="bg-yellow-50 rounded-lg p-6 mb-8">
                <h4 class="font-semibold text-gray-900 mb-2">Avantages du photovoltaïque</h4>
                <ul class="text-gray-600 space-y-1">
                  <li>• Réduction significative de la facture électrique</li>
                  <li>• Énergie propre et renouvelable</li>
                  <li>• Retour sur investissement attractif</li>
                  <li>• Valorisation du patrimoine immobilier</li>
                </ul>
              </div>

              <div class="flex flex-col  mt-[5.9rem] gap-4">
                <button @click="requestQuote('Photovoltaïque')"
                  class="bg-yellow-600 text-white px-8 py-3 rounded-lg hover:bg-yellow-700 transition-colors font-medium">
                  Demander un devis
                </button>
                <button
                  class="border border-gray-300 text-gray-700  py-3 rounded-lg hover:bg-gray-50 transition-colors font-medium">
                  Calculer mes économies
                </button>
              </div>
            </div>
          </div>

          <!-- Maintenance & Dépannage -->
          <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
            <img src="/src/assets/Maintenance.jpg" alt="Maintenance" class="w-full h-40 object-cover rounded-t-2xl" />
            <div class="p-8 pt-5">
              <div class="flex items-center mb-6">
                <h2 class="text-2xl font-bold text-blue-950">Maintenance & Dépannage</h2>
              </div>

             <div class="mb-8">
    <Swiper
      :modules="modules"
      :slides-per-view="1"
      :space-between="20"
      :autoplay="{ delay: 4000, disableOnInteraction: false }" 
      :loop="true"
      :pagination="{ clickable: true }"
      class="w-full "
    >
      <!-- Slide 1 -->
      <SwiperSlide class=" mb-7">
        <div>
          <h3 class="text-xl font-semibold text-gray-900 mb-4">Maintenance Préventive</h3>
          <ul class="space-y-3 text-gray-600">
            <li class="flex items-start space-x-3">
              <svg class="w-5 h-5 text-green-600 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd"
                  d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                  clip-rule="evenodd"></path>
              </svg>
              <span>Contrôles périodiques programmés</span>
            </li>
            <li class="flex items-start space-x-3">
              <svg class="w-5 h-5 text-green-600 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd"
                  d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                  clip-rule="evenodd"></path>
              </svg>
              <span>Optimisation des performances</span>
            </li>
            <li class="flex items-start space-x-3">
              <svg class="w-5 h-5 text-green-600 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd"
                  d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                  clip-rule="evenodd"></path>
              </svg>
              <span>Prolongation de la durée de vie</span>
            </li>
            <li class="flex items-start space-x-3">
              <svg class="w-5 h-5 text-green-600 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd"
                  d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                  clip-rule="evenodd"></path>
              </svg>
              <span>Réduction des coûts d'exploitation</span>
            </li>
          </ul>
        </div>
      </SwiperSlide>

      <!-- Slide 2 -->
      <SwiperSlide  class=" mb-7">
        <div>
          <h3 class="text-xl font-semibold text-gray-900 mb-4">Dépannage d'Urgence</h3>
          <ul class="space-y-3 text-gray-600">
            <li class="flex items-start space-x-3">
              <svg class="w-5 h-5 text-green-600 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd"
                  d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                  clip-rule="evenodd"></path>
              </svg>
              <span>Intervention rapide 24h/24</span>
            </li>
            <li class="flex items-start space-x-3">
              <svg class="w-5 h-5 text-green-600 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd"
                  d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                  clip-rule="evenodd"></path>
              </svg>
              <span>Diagnostic précis des pannes</span>
            </li>
            <li class="flex items-start space-x-3">
              <svg class="w-5 h-5 text-green-600 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd"
                  d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                  clip-rule="evenodd"></path>
              </svg>
              <span>Réparations durables</span>
            </li>
            <li class="flex items-start space-x-3">
              <svg class="w-5 h-5 text-green-600 mt-0.5" fill="currentColor" viewBox="0 0 20 20">
                <path fill-rule="evenodd"
                  d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                  clip-rule="evenodd"></path>
              </svg>
              <span>Remise en service immédiate</span>
            </li>
          </ul>
        </div>
      </SwiperSlide>
    </Swiper>

    <!-- pagination dots -->
    <div class="swiper-pagination mt-6"></div>
  </div>

              <div class="bg-green-50 rounded-lg p-6 mb-8">
                <div class="flex items-center mb-3">
                  <svg class="w-6 h-6 text-green-600 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                  </svg>
                  <h4 class="font-semibold text-gray-900">Service d'urgence 24h/24</h4>
                </div>
                <p class="text-gray-600">Notre équipe d'intervention est disponible en permanence pour résoudre vos
                  pannes électriques et pneumatiques dans les plus brefs délais.</p>
              </div>

              <div class="flex flex-col  gap-4">
                <button @click="requestQuote('Maintenance')"
                  class="bg-green-600 text-white px-8 py-3 rounded-lg hover:bg-green-700 transition-colors font-medium">
                  Demander un devis
                </button>
                <button
                  class="border border-gray-300 text-gray-700 px-8 py-3 rounded-lg hover:bg-gray-50 transition-colors font-medium">
                  Urgence 24h/24
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- CTA Section -->
    <section class="bg-blue-600 py-16">
      <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h2 class="text-3xl font-bold text-white mb-4">Prêt à démarrer votre projet ?</h2>
        <p class="text-xl text-blue-100 mb-8">
          Obtenez un devis gratuit et personnalisé pour vos besoins en électricité, pneumatique ou photovoltaïque
        </p>
        <div class="flex flex-col sm:flex-row gap-4 justify-center">
          <button @click="requestQuote('Général')"
            class="bg-white text-blue-600 px-8 py-4 rounded-lg hover:bg-gray-50 transition-colors font-semibold text-lg">
            Demander un devis gratuit
          </button>
          <button
            class="border-2 border-white text-white px-8 py-4 rounded-lg hover:bg-white hover:text-blue-600 transition-colors font-semibold text-lg">
            Nous contacter
          </button>
        </div>
      </div>
    </section>
    <Footer />

    <!-- Quote Modal -->
    <div v-if="showQuoteModal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 z-50">
      <div class="bg-white rounded-2xl max-w-md w-full p-6">
        <div class="flex justify-between items-center mb-4">
          <h3 class="text-xl font-bold text-gray-900">Demander un devis</h3>
          <button @click="showQuoteModal = false" class="text-gray-400 hover:text-gray-600">
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
            </svg>
          </button>
        </div>
        <form @submit.prevent="submitQuote" class="space-y-5 bg-white p-6 rounded-2xl shadow-lg">
  <!-- Service -->
  <div>
    <label class="block text-sm font-medium text-gray-700 mb-1">Service</label>
    <input 
      v-model="quoteForm.service" 
      type="text" 
      readonly
      class="w-full px-4 py-3 border border-gray-300 rounded-xl bg-gray-100 text-gray-600"
    >
  </div>

  <!-- Subservice (dropdown) -->
<div class="relative">
  <label for="subservice" class="block text-sm font-semibold text-gray-700 mb-2">
    Sous-service
  </label>

  <select
    v-model="quoteForm.subservice"
    id="subservice"
    class="w-full appearance-none px-4 py-3 pr-10 rounded-xl border border-gray-300 
           focus:ring-2 focus:ring-blue-500 
           bg-white shadow-sm text-gray-700 text-sm transition duration-150 ease-in-out"
  >
    <option disabled value="">-- Choisir un sous-service --</option>
    <option 
      v-for="item in serviceitems" 
      :key="item" 
      :value="item"
      class="py-2"
    >
      {{ item }}
    </option>
  </select>

  <!-- Custom arrow -->
  <svg 
    class="absolute right-3 top-10 w-5 h-5 text-gray-400 pointer-events-none" 
    xmlns="http://www.w3.org/2000/svg" 
    fill="none" viewBox="0 0 24 24" stroke="currentColor">
    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
  </svg>
</div>


  <!-- Nom complet -->
  <div>
    <label class="block text-sm font-medium text-gray-700 mb-1">Nom complet</label>
    <input 
      v-model="quoteForm.name" 
      type="text" 
      required
      class="w-full px-4 py-3 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-500 focus:border-transparent"
    >
  </div>

  <!-- Email -->
  <div>
    <label class="block text-sm font-medium text-gray-700 mb-1">Email</label>
    <input 
      v-model="quoteForm.email" 
      type="email" 
      required
      class="w-full px-4 py-3 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-500 focus:border-transparent"
    >
  </div>

  <!-- Téléphone -->
  <div>
    <label class="block text-sm font-medium text-gray-700 mb-1">Téléphone</label>
    <input 
      v-model="quoteForm.phone" 
      type="tel" 
      required
      class="w-full px-4 py-3 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-500 focus:border-transparent"
    >
  </div>

  <!-- Submit button -->
  <button 
    type="submit"
    class="w-full bg-gradient-to-r from-green-500 to-blue-600 text-white py-3 rounded-xl hover:opacity-90 transition-all font-semibold shadow-md"
  >
    Envoyer la demande
  </button>
</form>

      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, reactive } from 'vue'
import Header from '../../components/LayoutSociete/AppHeader.vue'
import Footer from '../../components/LayoutSociete/AppFooter.vue'
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Pagination, Autoplay } from 'swiper/modules';

// استيراد CSS ديال Swiper
import 'swiper/css';
import 'swiper/css/pagination';

const modules = [Pagination, Autoplay];
const showQuoteModal = ref(false)
const quoteForm = reactive({
  service: '',
  subservice:'',
  name: '',
  email: '',
  phone: '',
  message: ''
})

const serviceitems= ref([]);

const listsubServices=ref({
  secteurTertiare: ['Installations Électriques','Domotique','Câblage','Vidéosurveillance',"Systèmes d'Alarme",'Maintenance'],
  secteurIndustriel: ['Réseaux Électriques','Réseaux Pneumatiques','Armoires Électriques','Moteurs','Groupes Électrogènes','HTA (Haute Tension)','Sécurité Incendie'],
  Photovoltaïque: ['Étude','Installation','Maintenance'],
  Maintenance: ['Maintenance Préventive',"Dépannage d'Urgence"],

})

const requestQuote = (service) => {
  quoteForm.service = service
  if(service==='Secteur Tertiaire'){
    serviceitems.value= listsubServices.value.secteurTertiare
    quoteForm.subservice= serviceitems.value[0]
    console.log(serviceitems.value[0]);
    
  }else if(service==='Secteur Industriel'){
    serviceitems.value=listsubServices.value.secteurIndustriel
    quoteForm.subservice= serviceitems.value[0]
    console.log(serviceitems.value[0]);
  }else if(service==='Photovoltaïque'){
    serviceitems.value=listsubServices.value.Photovoltaïque
    quoteForm.subservice= serviceitems.value[0]
    console.log(serviceitems.value[0]);
  }else{
    serviceitems.value=listsubServices.value.Maintenance
    quoteForm.subservice= serviceitems.value[0]
    console.log(serviceitems.value[0]);
  }
  showQuoteModal.value = true
}

const submitQuote = () => {
  // Here you would typically send the form data to your backend
  console.log('Quote request submitted:', quoteForm)
  alert('Votre demande de devis a été envoyée avec succès ! Nous vous contacterons dans les plus brefs délais.')
  showQuoteModal.value = false

  // Reset form
  Object.assign(quoteForm, {
    service: '',
    name: '',
    email: '',
    phone: '',
    message: ''
  })

  const services = [
    {
      title: "Secteur Tertaire",
      image: "/src/assets/Tertaire.jpg", // <-- ajoute ton image ici
      items: [
        "Installations électriques",
        "Domotique",
        "Câblage",
        "Vidéosurveillance",
        "Alarme",
        "Maintenance",
      ],
    },
    {
      title: "Secteur Industrielle",
      image: "/src/assets/Industrielle.jpg",
      items: [
        "Réseaux électriques",
        "Pneumatiques",
        "Armoires électriques",
        "Moteurs",
        "Groupes électrogènes",
        "Sécurité incendie",
      ],
    },
    {
      title: "Photovoltaïque & Énergie renouvelable",
      image: "/src/assets/Photovoltaïque.jpgpng",
      items: ["Étude", "Installation", "Maintenance"],
    },
    {
      title: "Maintenance & Dépannage",
      image: "/src/assets/Maintenance.jpg",
      items: [
        "Compresseurs",
        "Réseaux d'air",
        "Vérins pneumatiques",
        "Maintenance",
      ],
    },
  ];
}
</script>