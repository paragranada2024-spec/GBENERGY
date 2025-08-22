<template>
  <div class="min-h-screen bg-gray-50">
    <!-- Hero Section -->
     <Header/>
    <section class="bg-gradient-to-r from-blue-600 to-blue-700 text-white py-16">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h1 class="text-4xl md:text-5xl font-bold mb-6">Contactez-nous</h1>
        <p class="text-xl md:text-2xl mb-8 text-blue-100">
          Obtenez votre devis gratuit dès aujourd'hui
        </p>
        <div class="inline-flex items-center bg-white text-blue-600 px-6 py-3 rounded-lg font-semibold">
          <svg class="w-5 h-5 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path>
          </svg>
          Réponse sous 24h garantie
        </div>
      </div>
    </section>

    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
      <div class="grid lg:grid-cols-2 gap-16">
        <!-- Contact Information -->
        <div class="space-y-8">
          <div>
            <h2 class="text-3xl font-bold text-gray-900 mb-8">Nos Coordonnées</h2>
            
            <!-- Contact Cards -->
            <div class="space-y-6">
              <!-- Phone -->
              <div class="bg-white p-6 rounded-xl shadow-lg border border-gray-100 hover:shadow-xl transition-shadow">
                <div class="flex items-start space-x-4">
                  <div class="bg-blue-100 p-3 rounded-lg">
                    <svg class="w-6 h-6 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path>
                    </svg>
                  </div>
                  <div>
                    <h3 class="text-lg font-semibold text-gray-900 mb-1">Téléphone</h3>
                    <p class="text-gray-600 mb-2">Appelez-nous pour un devis immédiat</p>
                    <a href="tel:+212123456789" class="text-blue-600 font-semibold hover:text-blue-700 text-lg">
                      +212 123 456 789
                    </a>
                  </div>
                </div>
              </div>

              <!-- Email -->
              <div class="bg-white p-6 rounded-xl shadow-lg border border-gray-100 hover:shadow-xl transition-shadow">
                <div class="flex items-start space-x-4">
                  <div class="bg-blue-100 p-3 rounded-lg">
                    <svg class="w-6 h-6 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
                    </svg>
                  </div>
                  <div>
                    <h3 class="text-lg font-semibold text-gray-900 mb-1">Email</h3>
                    <p class="text-gray-600 mb-2">Envoyez-nous votre demande</p>
                    <a href="mailto:contact@gbenergy.ma" class="text-blue-600 font-semibold hover:text-blue-700">
                      contact@gbenergy.ma
                    </a>
                  </div>
                </div>
              </div>

              <!-- Address -->
              <div class="bg-white p-6 rounded-xl shadow-lg border border-gray-100 hover:shadow-xl transition-shadow">
                <div class="flex items-start space-x-4">
                  <div class="bg-blue-100 p-3 rounded-lg">
                    <svg class="w-6 h-6 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"></path>
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path>
                    </svg>
                  </div>
                  <div>
                    <h3 class="text-lg font-semibold text-gray-900 mb-1">Adresse</h3>
                    <p class="text-gray-600 mb-2">Visitez notre bureau</p>
                    <p class="text-gray-800">
                      123 Avenue Mohammed V<br>
                      Casablanca, Maroc<br>
                      20000
                    </p>
                  </div>
                </div>
              </div>
            </div>

            <!-- Business Hours -->
            <div class="bg-blue-50 p-6 rounded-xl mt-8">
              <h3 class="text-lg font-semibold text-gray-900 mb-4">Horaires d'ouverture</h3>
              <div class="space-y-2 text-gray-700">
                <div class="flex justify-between">
                  <span>Lundi - Vendredi</span>
                  <span class="font-medium">8h00 - 18h00</span>
                </div>
                <div class="flex justify-between">
                  <span>Samedi</span>
                  <span class="font-medium">8h00 - 13h00</span>
                </div>
                <div class="flex justify-between">
                  <span>Dimanche</span>
                  <span class="font-medium text-red-600">Fermé</span>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Quote Request Form -->
        <div class="bg-white p-8 rounded-2xl shadow-xl border border-gray-100">
          <div class="text-center mb-8">
            <h2 class="text-3xl font-bold text-gray-900 mb-4">Obtenez votre devis gratuit</h2>
            <p class="text-gray-600">Remplissez le formulaire ci-dessous et nous vous contacterons sous 24h</p>
          </div>

          <form @submit.prevent="submitQuote" class="space-y-6">
            <!-- Name -->
            <div>
              <label for="name" class="block text-sm font-semibold text-gray-700 mb-2">
                Nom complet *
              </label>
              <input
                type="text"
                id="name"
                v-model="form.name"
                required
                class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors"
                placeholder="Votre nom complet"
              >
            </div>

            <!-- Email -->
            <div>
              <label for="email" class="block text-sm font-semibold text-gray-700 mb-2">
                Email *
              </label>
              <input
                type="email"
                id="email"
                v-model="form.email"
                required
                class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors"
                placeholder="votre@email.com"
              >
            </div>

            <!-- Phone -->
            <div>
              <label for="phone" class="block text-sm font-semibold text-gray-700 mb-2">
                Téléphone *
              </label>
              <input
                type="tel"
                id="phone"
                v-model="form.phone"
                required
                class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors"
                placeholder="+212 123 456 789"
              >
            </div>

            <!-- Service Type -->
            <div>
              <label for="service" class="block text-sm font-semibold text-gray-700 mb-2">
                Type de service *
              </label>
              <select
                id="service"
                v-model="form.service"
                required
                class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors"
              >
                <option value="">Sélectionnez un service</option>
                <option value="electricite-tertiaire">Électricité Tertiaire</option>
                <option value="electricite-industrielle">Électricité Industrielle</option>
                <option value="photovoltaique">Photovoltaïque & Énergie Renouvelable</option>
                <option value="pneumatique">Pneumatique</option>
                <option value="maintenance">Maintenance & Dépannage</option>
                <option value="location">Location d'équipements</option>
                <option value="produits">Vente de produits</option>
                <option value="autre">Autre</option>
              </select>
            </div>

            <!-- Message -->
            <div>
              <label for="message" class="block text-sm font-semibold text-gray-700 mb-2">
                Décrivez votre projet *
              </label>
              <textarea
                id="message"
                v-model="form.message"
                required
                rows="4"
                class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors resize-none"
                placeholder="Décrivez votre projet, vos besoins, la superficie, le délai souhaité..."
              ></textarea>
            </div>

            <!-- Submit Button -->
            <button
              type="submit"
              :disabled="isSubmitting"
              class="w-full bg-blue-600 hover:bg-blue-700 disabled:bg-blue-400 text-white font-bold py-4 px-6 rounded-lg transition-colors flex items-center justify-center space-x-2"
            >
              <svg v-if="isSubmitting" class="animate-spin w-5 h-5" fill="none" viewBox="0 0 24 24">
                <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
                <path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
              </svg>
              <span>{{ isSubmitting ? 'Envoi en cours...' : 'Obtenez votre devis gratuit' }}</span>
            </button>

            <p class="text-sm text-gray-500 text-center">
              * Champs obligatoires. Vos données sont protégées et ne seront jamais partagées.
            </p>
          </form>

          <!-- Success Message -->
          <div v-if="showSuccess" class="mt-6 p-4 bg-green-50 border border-green-200 rounded-lg">
            <div class="flex items-center space-x-2">
              <svg class="w-5 h-5 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
              </svg>
              <p class="text-green-800 font-medium">
                Merci ! Votre demande a été envoyée. Nous vous contacterons sous 24h.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
<!-- Google Maps -->
          <div class="max-w-7xl m-auto mb-3">
            <h3 class="text-2xl font-bold text-gray-900 mb-4">Notre Localisation</h3>
            <div class="bg-white rounded-xl shadow-lg overflow-hidden">
              <iframe 
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3323.0969470094!2d-7.589843!3d33.5731104!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zMzPCsDM0JzIzLjIiTiA3wrAzNScyMy40Ilc!5e0!3m2!1sen!2sma!4v1234567890"
                width="100%" 
                height="300" 
                style="border:0;" 
                allowfullscreen="" 
                loading="lazy" 
                referrerpolicy="no-referrer-when-downgrade"
                class="w-full">
              </iframe>
            </div>
          </div>
    <!-- CTA Section -->
    <section class="bg-gradient-to-r from-blue-600 to-blue-700 text-white py-16">
      <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h2 class="text-3xl md:text-4xl font-bold mb-6">
          Prêt à démarrer votre projet ?
        </h2>
        <p class="text-xl text-gray-300 mb-8">
          Nos experts sont à votre disposition pour étudier vos besoins et vous proposer la meilleure solution.
        </p>
        <div class="flex flex-col sm:flex-row gap-4 justify-center">
          <a
            href="tel:+212123456789"
            class="bg-blue-600 hover:bg-blue-700 text-white font-bold py-4 px-8 rounded-lg transition-colors inline-flex items-center justify-center space-x-2"
          >
            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path>
            </svg>
            <span>Appelez maintenant</span>
          </a>
          <a
            href="mailto:contact@gbenergy.ma"
            class="bg-transparent border-2 border-white hover:bg-white hover:text-gray-900 text-white font-bold py-4 px-8 rounded-lg transition-colors inline-flex items-center justify-center space-x-2"
          >
            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
            </svg>
            <span>Envoyez un email</span>
          </a>
        </div>
      </div>
    </section>
    <Footer />
  </div>
</template>

<script setup>
import { ref, reactive } from 'vue'
import Header from '../../components/LayoutSociete/AppHeader.vue'
import Footer from '../../components/LayoutSociete/AppFooter.vue'
// Form data
const form = reactive({
  name: '',
  email: '',
  phone: '',
  service: '',
  message: ''
})

// Form state
const isSubmitting = ref(false)
const showSuccess = ref(false)

// Submit form
const submitQuote = async () => {
  isSubmitting.value = true
  
  try {
    // Simulate API call
    await new Promise(resolve => setTimeout(resolve, 1500))
    
    // Reset form
    Object.keys(form).forEach(key => {
      form[key] = ''
    })
    
    // Show success message
    showSuccess.value = true
    
    // Hide success message after 5 seconds
    setTimeout(() => {
      showSuccess.value = false
    }, 5000)
    
  } catch (error) {
    console.error('Error submitting form:', error)
  } finally {
    isSubmitting.value = false
  }
}
</script>