<script setup>
defineProps({
  label: {
    type: String,
    default: 'Space',
  },
  backgroundImage: {
    type: String,
    default: 'https://picsum.photos/200',
  },
})
</script>

<template>
  <div class="relative w-28 h-28 rounded bg-linear-to-r from-cyan-400 via-blue-400 to-indigo-400">
    <div class="width-full height-full p-1 rounded overflow-hidden absolute top-0 left-0 z-10">
      <img :src="backgroundImage" alt="background" class="w-full h-full object-cover rounded" />
    </div>
    <div class="absolute bottom-1 left-1.5 z-20">{{ label }}</div>
  </div>
</template>
