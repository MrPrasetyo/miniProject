<script setup>
import Hero from "@/components/Hero.vue";
import Homecards from "@/components/Homecards.vue";
import JobListings from "@/components/JobListings.vue";
</script>

<template>
  <Hero
    title="I want to Become Frontend Dev"
    subtitle="I Hope this all go right side"
  />
  <Homecards />
  <JobListings :limit="3" :show-button="true" />
</template>
