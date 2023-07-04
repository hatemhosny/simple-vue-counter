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
    class="text-md font-medium bg-gray-500 hover:bg-gray-600 transition py-1 px-4 text-white rounded drop-shadow-xl"
  >
    {{ title }}
  </button>
</template>
