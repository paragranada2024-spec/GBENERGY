<template>
  <div class="min-h-screen bg-gray-50">
    <!-- Navigation -->
    <nav class="bg-white shadow-sm border-b">
      <div class="max-w-6xl mx-auto px-6">
        <div class="flex justify-between items-center h-16">
          <div class="flex items-center">
            <router-link to="/" class="text-2xl font-bold text-blue-600">
              GB ENERGY
            </router-link>
          </div>
          <div class="hidden md:flex space-x-8">
            <router-link to="/" class="text-gray-700 hover:text-blue-600 transition-colors">
              Accueil
            </router-link>
            <router-link to="/about" class="text-gray-700 hover:text-blue-600 transition-colors">
              À propos
            </router-link>
            <router-link to="/services" class="text-gray-700 hover:text-blue-600 transition-colors">
              Services
            </router-link>
            <router-link to="/contact" class="text-gray-700 hover:text-blue-600 transition-colors">
              Contact
            </router-link>
          </div>
        </div>
      </div>
    </nav>

    <!-- Main Content -->
    <slot />

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
      <div class="max-w-6xl mx-auto px-6">
        <div class="grid md:grid-cols-3 gap-8">
          <div>
            <h3 class="text-2xl font-bold text-blue-400 mb-4">GB ENERGY</h3>
            <p class="text-gray-300">
              Votre partenaire de confiance pour tous vos besoins énergétiques depuis 2018.
            </p>
          </div>
          <div>
            <h4 class="text-lg font-semibold mb-4">Liens rapides</h4>
            <ul class="space-y-2">
              <li><router-link to="/" class="text-gray-300 hover:text-blue-400 transition-colors">Accueil</router-link></li>
              <li><router-link to="/about" class="text-gray-300 hover:text-blue-400 transition-colors">À propos</router-link></li>
              <li><router-link to="/services" class="text-gray-300 hover:text-blue-400 transition-colors">Services</router-link></li>
              <li><router-link to="/contact" class="text-gray-300 hover:text-blue-400 transition-colors">Contact</router-link></li>
            </ul>
          </div>
          <div>
            <h4 class="text-lg font-semibold mb-4">Contact</h4>
            <p class="text-gray-300">
              Email: contact@gb-energy.com<br>
              Téléphone: +33 1 23 45 67 89
            </p>
          </div>
        </div>
        <div class="border-t border-gray-800 mt-8 pt-8 text-center">
          <p class="text-gray-400">&copy; 2024 GB ENERGY. Tous droits réservés.</p>
        </div>
      </div>
    </footer>
  </div>
</template>
