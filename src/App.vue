<script setup lang="ts">
import { RouterView } from 'vue-router'
import { usePreferredDark } from '@vueuse/core'

const isDarkMode = usePreferredDark()
</script>

<template>
  <div class="min-w-svw min-h-svh bg-background text-foreground p-2 lg:p-4" :class="{ dark: isDarkMode }">
    <header></header>

    <RouterView />
  </div>
</template>

<style scoped></style>
