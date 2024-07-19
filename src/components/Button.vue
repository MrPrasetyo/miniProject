<script setup>
import { defineProps } from "vue";
import { RouterLink } from "vue-router";

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
  <RouterLink
    :to="website"
    :class="`inline-block ${bg} text-white rounded-lg px-4 py-2 hover:bg-gray-700`"
  >
    {{ buttonName }}
  </RouterLink>
</template>
