<template>
  <header class="w-full h-18 border-b border-gray-200 dark:border-gray-700 backColor backdrop-blur-md">
    <div class="h-full px-3 sm:px-4 md:px-6 max-w-7xl mx-auto flex items-center justify-between">
      <!-- Logo / Title -->
      <NuxtLink to="/" class="text-2xl font-semibold tracking-wide hover:opacity-80 transition-opacity">
        Hussain
      </NuxtLink>

      <!-- Navigation -->
      <nav class="hidden md:flex items-center gap-6 h-full">
        <NuxtLink
          v-for="(nav, index) in navigationBar"
          :key="index"
          :to="nav.path"
          class="text-gray-700 dark:text-gray-200 hover:text-black dark:hover:text-white transition-colors font-medium"
        >
          {{ nav.name }}
        </NuxtLink>
      </nav>

      <!-- Actions -->
      <div class="flex items-center gap-4">
        <CommonDarkLightMode />
        <CommonMultiLanguage />

        <button
          class="hidden font-sm font-medium xl:inline-block px-3 py-1.5 rounded-md cursor-pointer border border-gray-300 dark:border-gray-600 bg-transparent text-gray-700 dark:text-gray-200 hover:bg-black/80 hover:text-white dark:hover:bg-white/90 dark:hover:text-black transition-all duration-300"
        >
          Contact Us
        </button>
      </div>
    </div>
  </header>
</template>

<script setup lang="ts">
const navigationBar = reactive([
  { name: 'Home', path: '/' },
  { name: 'About', path: '/about' },
  { name: 'Services', path: '/services' },
  { name: 'Projects', path: '/projects' }
])
</script>

<style scoped>
</style>
