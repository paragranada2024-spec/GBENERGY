<template>
  <section id="contact" class="py-20 bg-white flex justify-center items-center">
    <div class="max-w-3xl w-full mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-10">
        <h2 class="text-3xl lg:text-4xl font-bold text-gray-900 mb-4">
          Contactez-nous
        </h2>
        <p class="text-xl text-gray-600">
          Prêt à démarrer votre projet ? Demandez votre devis gratuit
        </p>
      </div>
      
      <!-- Formulaire centré -->
      <div class="bg-gray-50 rounded-xl p-8 shadow-lg">
        <form @submit.prevent="submitForm" class="space-y-6">
          
          <!-- Nom -->
          <div>
            <label for="name" class="block text-sm font-medium text-gray-700 mb-2">
              Nom complet *
            </label>
            <input
              v-model="form.name"
              type="text"
              id="name"
              required
              class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-colors"
              placeholder="Votre nom complet"
            />
          </div>
          
          <!-- Email -->
          <div>
            <label for="email" class="block text-sm font-medium text-gray-700 mb-2">
              Email *
            </label>
            <input
              v-model="form.email"
              type="email"
              id="email"
              required
              class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-colors"
              placeholder="votre@email.com"
            />
          </div>
          
          <!-- Téléphone -->
          <div>
            <label for="phone" class="block text-sm font-medium text-gray-700 mb-2">
              Téléphone *
            </label>
            <input
              v-model="form.phone"
              type="tel"
              id="phone"
              required
              class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-colors"
              placeholder="+212 6XX XXX XXX"
            />
          </div>

          <!-- Choix du service -->
          <div>
            <label for="service" class="block text-sm font-medium text-gray-700 mb-2">
              Service souhaité *
            </label>
            <select
              v-model="form.service"
              id="service"
              required
              class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent transition-colors"
            >
              <option value="" disabled>-- Sélectionnez un service --</option>
              <option value="tertiaire">Électricité Tertiaire</option>
              <option value="industriel">Électricité Industrielle</option>
              <option value="photovoltaïque">Photovoltaïque & Énergie renouvelable</option>
              <option value="maintenance">Maintenance & Dépannage</option>
            </select>
          </div>
          
          <!-- Bouton -->
          <button
            type="submit"
            :disabled="isSubmitting"
            class="w-full bg-blue-600 text-white px-6 py-4 rounded-lg text-lg font-semibold hover:bg-blue-700 disabled:opacity-50 disabled:cursor-not-allowed transition-all duration-300 shadow-lg hover:shadow-xl"
          >
            <span v-if="!isSubmitting">Envoyer ma demande</span>
            <span v-else class="flex items-center justify-center">
              <svg class="animate-spin -ml-1 mr-3 h-5 w-5 text-white" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24">
                <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
                <path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
              </svg>
              Envoi en cours...
            </span>
          </button>
        </form>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, reactive } from 'vue'

const isSubmitting = ref(false)

const form = reactive({
  name: '',
  email: '',
  phone: '',
  service: '' // <-- Nouveau champ ajouté
})

const submitForm = async () => {
  isSubmitting.value = true
  
  // Simulation d'envoi
  await new Promise(resolve => setTimeout(resolve, 2000))
  
  alert(`Merci ${form.name} pour votre demande concernant "${form.service}" ! Nous vous contacterons sous 24h.`)
  
  // Reset form
  Object.assign(form, {
    name: '',
    email: '',
    phone: '',
    service: ''
  })
  isSubmitting.value = false
}
</script>
