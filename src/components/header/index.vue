<!-- components/BaseNav.vue -->
<template>
  <nav class="bg-slate-900 text-gray-300">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center h-16">
        <div class="text-xl font-bold text-white">Textify</div>

        <!-- Right: Navigation Links -->
        <ul class="flex space-x-6">
          <li v-for="item in navItems" :key="item.name">
            <RouterLink
              :to="item.path"
              class="hover:text-white transition"
              active-class="text-white font-medium"
              exact-active-class="text-white font-medium"
            >
              {{ item.name }}
            </RouterLink>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { RouterLink } from 'vue-router'

const navItems = [
  { name: 'Home', path: '/' },
  { name: 'About', path: '/about' },
  { name: 'Story', path: '/story' },
  { name: 'Contact', path: '/contact' },
]
</script>
