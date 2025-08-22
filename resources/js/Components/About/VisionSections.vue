<template>
  <section class="bg-white rounded-lg shadow-sm p-8 md:p-12">
    <div class="text-center mb-12">
      <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">Notre Vision</h2>
      <div class="w-24 h-1 bg-blue-600 mx-auto"></div>
    </div>

   <div class="max-w-4xl mx-auto">
    
  <div class="text-center mb-12">
    <div class=" flex items-center justify-center mx-10 mb-6">
      <!-- Remplacer l'icône par une image -->
      <img src="/storage/images/image13.png" alt="Icone" class="w-[1150] h-80 rounded-xl object-contain" />
    </div>
    <h3 class="text-2xl font-bold text-gray-900 mb-4">Construire des relations de confiance durables</h3>
    <p class="text-lg text-gray-700 leading-relaxed">
      Notre vision est de développer des partenariats solides et pérennes avec nos clients, basés sur la confiance
      mutuelle, la transparence et l'excellence de nos services.
    </p>
  </div>



      <div class="grid md:grid-cols-2 gap-8">
        <div class="flex items-start space-x-4">
          <div class="bg-blue-100 w-12 h-12 rounded-full flex items-center justify-center flex-shrink-0">
            <Handshake class="w-6 h-6 text-blue-600" />
          </div>
          <div>
            <h4 class="text-xl font-semibold text-gray-900 mb-2">Partenariat à long terme</h4>
            <p class="text-gray-600">
              Nous privilégions les relations durables plutôt que les transactions ponctuelles, en accompagnant nos
              clients dans leur développement.
            </p>
          </div>
        </div>

        <div class="flex items-start space-x-4">
          <div class="bg-blue-100 w-12 h-12 rounded-full flex items-center justify-center flex-shrink-0">
            <TrendingUp class="w-6 h-6 text-blue-600" />
          </div>
          <div>
            <h4 class="text-xl font-semibold text-gray-900 mb-2">Croissance mutuelle</h4>
            <p class="text-gray-600">
              Votre succès est notre succès. Nous nous engageons à contribuer activement à la réussite de vos projets
              énergétiques.
            </p>
          </div>
        </div>
      </div>

      <div class="mt-12 p-6 bg-blue-50 rounded-lg">
        <blockquote class="text-center">
          <p class="text-lg text-gray-800 italic mb-4">
            "Chez GB ENERGY, nous croyons que la confiance se construit jour après jour, projet après projet. C'est
            cette philosophie qui guide toutes nos actions."
          </p>
          <footer class="text-blue-600 font-semibold">— L'équipe GB ENERGY</footer>
        </blockquote>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Heart, Handshake, TrendingUp } from 'lucide-vue-next'
</script>
