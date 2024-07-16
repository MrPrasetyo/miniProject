<script setup>
import { defineProps } from "vue";

defineProps({
  bg: {
    type: String,
    default: "bg-black",
  },
  buttonName: String,
  website: String,
});
</script>

<template>
  <a :href="website" :class="`inline-block ${bg} text-white rounded-lg px-4 py-2 hover:bg-gray-700`" target="_blank"> {{buttonName}} </a>
</template>
