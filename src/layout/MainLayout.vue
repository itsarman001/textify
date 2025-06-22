<template>
  <main class="bg-slate-950 text-slate-100 min-h-screen flex flex-col">
    <header>
      <Nav />
    </header>

    <div class="flex-1">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-6">
        <slot></slot>
      </div>
    </div>

    <footer>
      <Footer />
    </footer>
  </main>
</template>

<script setup>
import Nav from '../components/header/index.vue'
import Footer from '../components/footer/index.vue'
</script>
