<script setup>
import BaseHeader from "../components/BaseHeader.vue";
</script>

<template>
  <div class="relative">
    <img
      class="h-screen w-full absolute top-0 left-0 z-0"
      src="/sunset.jpg"
      alt="background"
    />
    <div
      class="h-screen p-8 absolute z-10 top-0 left-0 bg-transparent text-slate-400"
    >
      <BaseHeader />
    </div>
  </div>
</template>
