<template>
  <div class="relative">
    <!-- Trigger -->
    <div
class="flex items-center gap-1 py-3 px-2 cursor-pointer select-none
             text-gray-700 dark:text-gray-200 hover:text-black dark:hover:text-white transition"
      @mouseenter="showLangMenu = true" @mouseleave="showLangMenu = false">
      <Icon name="ic:round-language" size="1.6rem" />
      <span class="text-sm font-semibold">{{ selectedLanguage }}</span>
    </div>

    <!-- Dropdown -->

    <div
v-if="showLangMenu" class="absolute top-full right-0 w-36 rounded-xl shadow-lg border
               bg-white/80 dark:bg-[#1e1e1e]/80 backdrop-blur-md
               border-gray-200 dark:border-gray-700
               overflow-hidden z-50" @mouseenter="showLangMenu = true" @mouseleave="showLangMenu = false">
      <button
class="w-full text-left px-4 py-2 text-sm font-medium  
                 text-gray-700 dark:text-gray-200 
                 hover:bg-gray-100 dark:hover:bg-gray-800 transition" @click="selectLang('AR')">
        Arabic
      </button>

      <button
class="w-full text-left px-4 py-2 text-sm font-medium  
                 text-gray-700 dark:text-gray-200 
                 hover:bg-gray-100 dark:hover:bg-gray-800 transition" @click="selectLang('ENG')">
        English
      </button>
    </div>
  </div>
</template>

<script setup lang="ts">
const showLangMenu = ref(false)
const selectedLanguage = ref<'ENG' | 'AR'>('ENG')

const selectLang = (lang: 'ENG' | 'AR') => {
  selectedLanguage.value = lang
  showLangMenu.value = false
}
</script>
