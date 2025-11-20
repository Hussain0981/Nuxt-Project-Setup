<template>
  <div class="cursor-pointer flex items-center" @click="toggleMode">
    <Icon
      :name="isDark.value === 'dark'
      ? 'material-symbols:light-mode-outline-rounded'
      : 'material-symbols:dark-mode-outline-rounded'" size="1.6rem" />
  </div>
</template>
<script setup lang="ts">
const isDark = useColorMode();

function toggleMode() {
  isDark.value = isDark.value === 'light' ? 'dark' : 'light';
}
</script>
