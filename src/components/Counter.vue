<script setup lang="ts">
import { ref } from "vue";
import PrimaryButton from "./PrimaryButton.vue";
import DangerButton from "./DangerButton.vue";

const count = ref(0);
</script>

<template>
  <div class="w-full mt-8 flex justify-center">
    <span ref="counter" class="text-3xl font-bold">{{ count }}</span>
  </div>
  <div class="w-full mt-4 flex flex-row space-x-4 justify-center">
    <primary-button ref="decrementButton" title="-" @click="count--" />
    <primary-button ref="incrementButton" title="+" @click="count++" />
  </div>
  <div class="w-full mt-4 flex flex-row space-x-4 justify-center">
    <danger-button ref="resetButton" title="Reset" @click="count = 0" />
  </div>
</template>
