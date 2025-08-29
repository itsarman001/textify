<script setup lang="ts">
import LayoutList from "./icons/LayoutList.vue";
</script>

<template>
  <header>
    <nav class="flex justify-between items-center w-full">
      <h2>Welcome back, Arman</h2>

      <div class="ms-auto flex gap-2">
        <button class="flex items-center gap-2 text-white px-4 py-2 rounded">
          <LayoutList color="white" />
          <span>Customize</span>
        </button>
      </div>
    </nav>
  </header>
</template>
