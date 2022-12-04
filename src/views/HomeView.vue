<script setup lang="ts">
import BeerCounter from "@/components/BeerCounter.vue";
</script>

<template>
  <main>
    <BeerCounter
      v-for="value in demoBeers"
      :beerName="value.name"
      :initialAmount="value.currentAmout"
      v-bind:key="value.name"
    />
  </main>
</template>

<script lang="ts">
import demoBeers from "../assets/demoBeers.json";

console.log(demoBeers);

export default {
  data() {
    return demoBeers;
  },
};
</script>
