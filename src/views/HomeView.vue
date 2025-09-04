<script setup lang="ts">
import { PaintbrushVertical } from 'lucide-vue-next'
</script>

<template>
  <main
    class="min-h-screen w-full px-4 sm:px-6 lg:px-8 py-6 bg-gradient-to-r from-gray-700 via-gray-900 to-black text-white"
  >
    <!-- Header -->
    <header class="flex items-center justify-between mb-6">
      <h2 class="text-xl sm:text-2xl font-semibold">Welcome, User</h2>

      <div>
        <div
          class="cursor-pointer rounded-full bg-gray-800/50 px-4 py-2 transition hover:bg-gray-800/70 flex items-center gap-2 text-sm sm:text-base"
        >
          <PaintbrushVertical :size="20" />
          <span>Customize</span>
        </div>
      </div>
    </header>

    <!-- Main Section -->
    <section class="flex flex-col lg:flex-row gap-6 mb-8">
      <div class="flex-1 bg-white/5 rounded-lg min-h-[200px] p-4">Main Content</div>
      <aside class="w-full lg:w-1/3 bg-white/5 rounded-lg min-h-[200px] p-4">Sidebar</aside>
    </section>

    <!-- Footer -->
    <footer class="text-sm text-gray-400 text-center mt-auto py-4">
      © 2025 - Your Custom New Tab
    </footer>
  </main>
</template>
