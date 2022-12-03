<script setup lang="ts">
import BeerCounter from "@/components/BeerCounter.vue";
</script>

<template>
  <main>
    <BeerCounter beerName="Polish Ale" :initialAmount="8" />
  </main>
</template>
