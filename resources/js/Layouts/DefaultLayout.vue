<template>
  <div class="min-h-screen bg-white">
    <AppHeader />
    <main>
      <slot />
    </main>
    <AppFooter />
  </div>
</template>

<script setup>
import AppHeader from '@/Components/LayoutSociete/AppHeader.vue'
import AppFooter from '@/Components/LayoutSociete/AppFooter.vue'
</script>