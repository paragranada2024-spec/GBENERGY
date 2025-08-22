<template>
  <div>
    <HeroSections />
    <ServicesSection />
    <TestimonialsSection />
    <ContactSection />
  </div>
</template>

<script setup>
import HeroSections from '@/Components/HeroSections.vue'
import ServicesSection from '@/Components/ServicesSection.vue'
import TestimonialsSection from '@/Components/TestimonialsSection.vue'
import ContactSection from '@/Components/ContactSection.vue'
import DefaultLayout from '@/Layouts/DefaultLayout.vue'

defineOptions({
  layout:DefaultLayout
})
</script>