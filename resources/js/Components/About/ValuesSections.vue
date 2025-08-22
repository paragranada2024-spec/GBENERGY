<template>
  <section>
    <!-- Title -->
    <div class="text-center mb-12">
      <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">Nos Valeurs</h2>
      <div class="w-24 h-1 bg-blue-600 mx-auto mb-6"></div>
      <p class="text-lg text-gray-600 max-w-2xl mx-auto">
        Les principes qui guident notre action au quotidien et font notre différence
      </p>
    </div>

    <!-- Cards -->
    <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
      <div 
        v-for="(value, index) in values" 
        :key="index" 
        class="bg-white rounded-lg shadow-sm overflow-hidden hover:shadow-md transition-shadow"
      >
        <!-- Image carré -->
        <div class="w-full h-40 bg-gray-100">
          <img 
            :src="value.image" 
            :alt="value.title" 
            class="w-full h-full object-cover"
          />
        </div>
        
        <!-- Content -->
        <div class="p-6 text-center">
          <h3 class="text-xl font-semibold text-gray-900 mb-3">{{ value.title }}</h3>
          <p class="text-gray-600 text-sm leading-relaxed">{{ value.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const values = [
  {
    image: "/storage/images/image8.png",
    title: "Compétence",
    description: "Une expertise technique pointue et une connaissance approfondie du secteur énergétique",
  },
  {
    image: "/storage/images/image9.png",
    title: "Rapidité",
    description: "Des interventions rapides et efficaces pour répondre à vos besoins dans les meilleurs délais",
  },
  {
    image: "/storage/images/image10.png",
    title: "Respect des délais",
    description: "Un engagement ferme sur les échéances avec une planification rigoureuse de nos projets",
  },
  {
    image: "/storage/images/image11.png",
    title: "Sécurité",
    description: "La sécurité est notre priorité absolue dans tous nos projets et interventions",
  },
]
</script>
