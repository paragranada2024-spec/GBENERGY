<template>
  <header class="bg-white shadow-sm border-b ">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center py-4 ">
        <!-- Logo -->
        <div class="flex items-center space-x-3">
          <div class="w-10 h-10 bg-blue-600 rounded-lg flex items-center justify-center">
            <span class="text-white font-bold text-lg">GB</span>
          </div>
          <span class="text-xl font-bold text-gray-900">GB ENERGY</span>
        </div>

        <!-- Navigation -->
        <nav class="hidden md:flex space-x-8">
          <a href="#" class="text-gray-600 hover:text-blue-600 transition-colors">Accueil</a>
          <a href="#" class="text-gray-600 hover:text-blue-600 transition-colors">Services</a>
          <a href="#" class="text-gray-600 hover:text-blue-600 transition-colors">Produits</a>
          <a href="#" class="text-gray-600 hover:text-blue-600 transition-colors">À propos</a>
          <a href="#" class="text-gray-600 hover:text-blue-600 transition-colors">Contact</a>
        </nav>

        <!-- CTA Button -->
        <div class=" hidden md:block ">
          <button class="bg-red-500 text-white px-6 py-2 rounded-lg hover:bg-red-700 transition-colors mr-3">
            Urgence 24h/24
          </button>
          <button @click="$emit('requestQuote')"
            class="bg-blue-600 text-white px-6 py-2 rounded-lg hover:bg-blue-700 transition-colors">
            Demander un devis
          </button>
        </div>

        <!-- Mobile Menu Button -->
        <button @click="toggleMobileMenu" class="md:hidden text-gray-600 hover:text-blue-600">
          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
          </svg>
        </button>
      </div>

      <!-- Mobile Menu -->
      <div v-if="showMobileMenu" class="md:hidden py-4 border-t">
        <nav class="flex flex-col text-center space-y-4">
          <a href="#" class="text-gray-600 hover:text-blue-600 transition-colors">Accueil</a>
          <a href="#" class="text-gray-600 hover:text-blue-600 transition-colors">Services</a>
          <a href="#" class="text-gray-600 hover:text-blue-600 transition-colors">Produits</a>
          <a href="#" class="text-gray-600 hover:text-blue-600 transition-colors">À propos</a>
          <a href="#" class="text-gray-600 hover:text-blue-600 transition-colors">Contact</a>
          <div class="">
          
            <button @click="$emit('requestQuote')"
              class="bg-blue-600 text-white px-6 w-full py-2 rounded-lg hover:bg-blue-700 transition-colors mb-3">
              Demander un devis
            </button>
              <button class="bg-red-500 text-white w-full px-6 py-2 rounded-lg hover:bg-red-700 transition-colors">
              Urgence 24h/24
            </button>
          </div>
        </nav>
      </div>
    </div>
  </header>
</template>

<script setup>
import { ref } from 'vue'

// Mobile menu state
const showMobileMenu = ref(false)

// Toggle mobile menu
const toggleMobileMenu = () => {
  showMobileMenu.value = !showMobileMenu.value
}

// Define emits
defineEmits(['requestQuote'])
</script>
