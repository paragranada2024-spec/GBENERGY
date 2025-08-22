<template>
  <section id="services" class="py-20 bg-gradient-to-br from-gray-50 to-blue-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-3xl lg:text-4xl font-bold text-gray-900 mb-4">
          Nos Services
        </h2>
        <p class="text-xl text-gray-600 max-w-3xl mx-auto">
          Des solutions complètes pour tous vos besoins énergétiques
        </p>
      </div>

      <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
        <div
          v-for="service in services"
          :key="service.title"
          class="bg-white rounded-xl shadow-lg hover:shadow-xl transition-all duration-300 group"
        >
          <!-- Image en haut -->
          <img
            v-if="service.image"
            :src="service.image"
            :alt="service.title"
            class="w-full h-40 object-cover rounded-t-2xl mb-4"
          />
          <div class="p-4">
            <!-- Titre -->
            <h3 class="text-xl font-semibold text-gray-900 mb-3">
              {{ service.title }}
            </h3>

            <!-- Description (optionnel si tu veux ajouter une petite phrase) -->
            <p v-if="service.description" class="text-gray-600 mb-4">
              {{ service.description }}
            </p>

            <!-- Liste des éléments -->
            <ul class="space-y-2">
              <li
                v-for="item in service.items"
                :key="item"
                class="flex items-center text-sm text-gray-600"
              >
                <svg
                  class="w-4 h-4 text-blue-600 mr-2"
                  fill="currentColor"
                  viewBox="0 0 20 20"
                >
                  <path
                    fill-rule="evenodd"
                    d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z"
                    clip-rule="evenodd"
                  />
                </svg>
                {{ item }}
              </li>
            </ul>
          </div>
        </div>
      </div>

      <div class="text-center mt-12">
        <a
          href="#contact"
          class="bg-blue-600 text-white px-2 py-4 rounded-lg text-lg font-semibold hover:bg-blue-700 transition-all duration-300 shadow-lg hover:shadow-xl md:px-6"
        >
          Demander un devis pour vos projets
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Zap, Factory, Sun, Wind } from "lucide-vue-next";

const services = [
  {
    title: "Secteur Tertaire",
    image: "/storage/images/image1.png", // <-- ajoute ton image ici
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
    image: "/storage/images/image2.png",
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
    image: "/storage/images/image3.png",
    items: ["Étude", "Installation", "Maintenance"],
  },
  {
    title: "Maintenance & Dépannage",
    image: "/storage/images/image4.png",
    items: [
      "Compresseurs",
      "Réseaux d'air",
      "Vérins pneumatiques",
      "Maintenance",
    ],
  },
];
</script>
