<!-- components/BaseFooter.vue -->
<template>
  <footer class="bg-slate-900 text-gray-400 text-sm py-4">
    <div
      class="max-w-7xl mx-auto px-4 flex flex-col sm:flex-row justify-between items-center space-y-2 sm:space-y-0"
    >
      <!-- Left: Brand -->
      <div class="font-semibold text-white">Textify</div>

      <!-- Center: Nav Links -->
      <nav class="flex space-x-4">
        <RouterLink
          v-for="item in navItems"
          :key="item.name"
          :to="item.path"
          class="hover:text-white transition"
          active-class="text-white font-medium"
          exact-active-class="text-white font-medium"
        >
          {{ item.name }}
        </RouterLink>
      </nav>
      <div>© {{ new Date().getFullYear() }} Textify</div>
    </div>
  </footer>
</template>

<script setup>
import { RouterLink } from 'vue-router'

const navItems = [
  { name: 'Home', path: '/' },
  { name: 'About', path: '/about' },
  { name: 'Contact', path: '/contact' },
]
</script>
