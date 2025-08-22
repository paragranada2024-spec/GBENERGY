<template>
    
  <div class="min-h-screen bg-gray-50">
    <!-- Hero Section -->
     <Header/>
    <section class="bg-gradient-to-r from-blue-600 to-blue-700 text-white py-20">
      <div class="max-w-6xl mx-auto px-4 text-center">
        <h1 class="text-4xl md:text-5xl font-bold mb-6">
          Produits & Location
        </h1>
        <p class="text-xl md:text-2xl mb-8 text-blue-100">
          Équipements de qualité et solutions de location pour tous vos projets
        </p>
        <button 
          @click="showQuoteModal = true"
          class="bg-white text-blue-600 px-8 py-4 rounded-lg font-semibold text-lg hover:bg-gray-100 transition-colors shadow-lg"
        >
          Demander un devis
        </button>
      </div>
    </section>

    <!-- Products Section -->
    <section class="py-20 bg-white">
      <div class="max-w-6xl mx-auto px-4">
        <div class="text-center mb-16">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4">
            Nos Produits
          </h2>
          <p class="text-xl text-gray-600 max-w-3xl mx-auto">
            Partenariat avec les plus grandes marques d'appareillages électriques et pneumatiques
          </p>
        </div>

        <div class="grid md:grid-cols-2 gap-12">
          <div>
            <h3 class="text-2xl font-bold text-gray-800 mb-6">
              Appareillages Électriques & Pneumatiques
            </h3>
            <div class="space-y-4">
              <div class="flex items-start gap-3">
                <div class="w-2 h-2 bg-blue-600 rounded-full mt-2 flex-shrink-0"></div>
                <p class="text-gray-700">
                  <strong>Équipements électriques :</strong> Disjoncteurs, contacteurs, relais, transformateurs, câbles et accessoires
                </p>
              </div>
              <div class="flex items-start gap-3">
                <div class="w-2 h-2 bg-blue-600 rounded-full mt-2 flex-shrink-0"></div>
                <p class="text-gray-700">
                  <strong>Systèmes pneumatiques :</strong> Vérins, distributeurs, régulateurs de pression, raccords et tuyauterie
                </p>
              </div>
              <div class="flex items-start gap-3">
                <div class="w-2 h-2 bg-blue-600 rounded-full mt-2 flex-shrink-0"></div>
                <p class="text-gray-700">
                  <strong>Marques partenaires :</strong> Schneider Electric, Legrand, ABB, Siemens, Festo, SMC
                </p>
              </div>
              <div class="flex items-start gap-3">
                <div class="w-2 h-2 bg-blue-600 rounded-full mt-2 flex-shrink-0"></div>
                <p class="text-gray-700">
                  <strong>Garantie qualité :</strong> Produits certifiés conformes aux normes internationales
                </p>
              </div>
            </div>
            <button 
              @click="showQuoteModal = true"
              class="mt-8 bg-blue-600 text-white px-6 py-3 rounded-lg font-semibold hover:bg-blue-700 transition-colors"
            >
              Demander un devis produits
            </button>
          </div>
          <div class="bg-gray-100 rounded-lg  text-center shadow-xl">
    <!-- Image -->
    <img src="/src/assets/image.png" alt="Équipements" class="mx-auto mb-4 w-full h-60 object-cover rounded-t-lg">
    
    <h4 class="text-xl font-bold text-gray-800 mb-4">Équipements Professionnels</h4>
    <p class="text-gray-600">
        Large gamme d'appareillages électriques et pneumatiques pour tous secteurs d'activité
    </p>
</div>

        </div>
      </div>
      
    </section>

    <!-- Rental Section -->
    <section class="py-20 bg-gray-50">
      <div class="max-w-6xl mx-auto px-4">
        <div class="text-center mb-16">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4">
            Services de Location
          </h2>
          <p class="text-xl text-gray-600 max-w-3xl mx-auto">
            Matériel professionnel en location pour vos chantiers et projets
          </p>
        </div>

        <div class="grid md:grid-cols-3 gap-8">
          <!-- Nacelles -->
          <div class="bg-white rounded-lg shadow-lg p-8 text-center hover:shadow-xl transition-shadow">
            <img src="/src/assets/Nacelles.jpg" alt="Maintenance" class=" max-h-[100px] w-full object-contain rounded-t-2xl mb-2" />
            <h3 class="text-xl font-bold text-gray-800 mb-4">Nacelles Élévatrices</h3>
            <ul class="text-gray-600 space-y-2 mb-6">
              <li>• Hauteurs de 8m à 30m</li>
              <li>• Nacelles ciseaux et articulées</li>
              <li>• Électriques et thermiques</li>
              <li>• Formation opérateur incluse</li>
            </ul>
            <button 
              @click="showQuoteModal = true"
              class="w-full bg-blue-600 text-white py-3 rounded-lg font-semibold hover:bg-blue-700 transition-colors"
            >
              Louer une nacelle
            </button>
          </div>

          <!-- Groupes électrogènes -->
          <div class="bg-white rounded-lg shadow-lg p-8 text-center hover:shadow-xl transition-shadow">
             <img src="/src/assets/Groupesélectrogènes.jpg" alt="Maintenance" class=" max-h-[100px] w-full object-contain rounded-t-2xl mb-2" />
            
            <h3 class="text-xl font-bold text-gray-800 mb-4">Groupes Électrogènes</h3>
            <ul class="text-gray-600 space-y-2 mb-6">
              <li>• Puissances de 5 à 500 kVA</li>
              <li>• Diesel et essence</li>
              <li>• Insonorisés disponibles</li>
              <li>• Livraison et installation</li>
            </ul>
            <button 
              @click="showQuoteModal = true"
              class="w-full bg-blue-600 text-white py-3 rounded-lg font-semibold hover:bg-blue-700 transition-colors"
            >
              Louer un groupe
            </button>
          </div>

          <!-- Chariots élévateurs -->
          <div class="bg-white rounded-lg shadow-lg p-8 text-center hover:shadow-xl transition-shadow">
             <img src="/src/assets/Chariotsélévateur.jpg" alt="Maintenance" class=" max-h-[100px] w-full object-contain rounded-t-2xl mb-2" />
            
            <h3 class="text-xl font-bold text-gray-800 mb-4">Chariots Élévateurs</h3>
            <ul class="text-gray-600 space-y-2 mb-6">
              <li>• Capacités de 1 à 5 tonnes</li>
              <li>• Électriques et thermiques</li>
              <li>• Tout-terrain disponibles</li>
              <li>• Maintenance incluse</li>
            </ul>
            <button 
              @click="showQuoteModal = true"
              class="w-full bg-blue-600 text-white py-3 rounded-lg font-semibold hover:bg-blue-700 transition-colors"
            >
              Louer un chariot
            </button>
          </div>
        </div>
      </div>
    </section>

    <!-- Advantages Section -->
    <section class="py-20 bg-white">
      <div class="max-w-6xl mx-auto px-4">
        <div class="text-center mb-16">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4">
            Pourquoi Choisir GB ENERGY ?
          </h2>
        </div>

        <div class="grid md:grid-cols-4 gap-8">
          <div class="text-center">
            <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-8 h-8 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path>
              </svg>
            </div>
            <h3 class="text-lg font-bold text-gray-800 mb-2">Qualité Garantie</h3>
            <p class="text-gray-600">Matériel certifié et régulièrement entretenu</p>
          </div>

          <div class="text-center">
            <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-8 h-8 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"></path>
              </svg>
            </div>
            <h3 class="text-lg font-bold text-gray-800 mb-2">Disponibilité 24/7</h3>
            <p class="text-gray-600">Service client et dépannage disponibles</p>
          </div>

          <div class="text-center">
            <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-8 h-8 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"></path>
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path>
              </svg>
            </div>
            <h3 class="text-lg font-bold text-gray-800 mb-2">Livraison Rapide</h3>
            <p class="text-gray-600">Livraison et installation sur site</p>
          </div>

          <div class="text-center">
            <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-8 h-8 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1"></path>
              </svg>
            </div>
            <h3 class="text-lg font-bold text-gray-800 mb-2">Prix Compétitifs</h3>
            <p class="text-gray-600">Tarifs transparents et adaptés</p>
          </div>
        </div>
      </div>
    </section>

    <!-- CTA Section -->
    <section class="py-20 bg-blue-600 text-white">
      <div class="max-w-4xl mx-auto px-4 text-center">
        <h2 class="text-3xl md:text-4xl font-bold mb-6">
          Besoin d'un Devis Personnalisé ?
        </h2>
        <p class="text-xl mb-8 text-blue-100">
          Contactez-nous pour obtenir un devis gratuit adapté à vos besoins
        </p>
        <button 
          @click="showQuoteModal = true"
          class="bg-white text-blue-600 px-8 py-4 rounded-lg font-semibold text-lg hover:bg-gray-100 transition-colors shadow-lg"
        >
          Obtenir mon devis gratuit
        </button>
      </div>
    </section>
    <Footer />

    <!-- Quote Modal -->
    <div v-if="showQuoteModal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center p-4 z-50">
      <div class="bg-white rounded-lg max-w-md w-full p-6">
        <div class="flex justify-between items-center mb-6">
          <h3 class="text-2xl font-bold text-gray-800">Demande de Devis</h3>
          <button @click="showQuoteModal = false" class="text-gray-500 hover:text-gray-700">
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
            </svg>
          </button>
        </div>
        
        <form @submit.prevent="submitQuote" class="space-y-4">
          <div>
            <label class="block text-sm font-medium text-gray-700 mb-1">Nom complet</label>
            <input v-model="form.name" type="text" required class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
          </div>
          
          <div>
            <label class="block text-sm font-medium text-gray-700 mb-1">Email</label>
            <input v-model="form.email" type="email" required class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
          </div>
          
          <div>
            <label class="block text-sm font-medium text-gray-700 mb-1">Téléphone</label>
            <input v-model="form.phone" type="tel" required class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
          </div>
          
          <div>
            <label class="block text-sm font-medium text-gray-700 mb-1">Type de besoin</label>
            <select v-model="form.serviceType" required class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent">
              <option value="">Sélectionnez...</option>
              <option value="produits">Achat de produits</option>
              <option value="location-nacelle">Location nacelle</option>
              <option value="location-groupe">Location groupe électrogène</option>
              <option value="location-chariot">Location chariot élévateur</option>
              <option value="autre">Autre</option>
            </select>
          </div>
          
          <div>
            <label class="block text-sm font-medium text-gray-700 mb-1">Message</label>
            <textarea v-model="form.message" rows="3" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Décrivez votre projet..."></textarea>
          </div>
          
          <button type="submit" class="w-full bg-blue-600 text-white py-3 rounded-lg font-semibold hover:bg-blue-700 transition-colors">
            Envoyer ma demande
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

const showQuoteModal = ref(false)

const form = reactive({
  name: '',
  email: '',
  phone: '',
  serviceType: '',
  message: ''
})

const submitQuote = () => {
  // Here you would typically send the form data to your backend
  console.log('Quote request submitted:', form)
  alert('Votre demande de devis a été envoyée avec succès ! Nous vous contacterons rapidement.')
  showQuoteModal.value = false
  
  // Reset form
  Object.keys(form).forEach(key => {
    form[key] = ''
  })
}
</script>