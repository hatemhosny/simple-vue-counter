<script setup lang="ts">
defineProps({
  title: {
    type: String,
    default: "Button",
  },
});
</script>

<template>
  <button
    class="text-md font-medium bg-red-500 hover:bg-red-600 transition py-1 px-4 text-white rounded drop-shadow-xl"
  >
    {{ title }}
  </button>
</template>
