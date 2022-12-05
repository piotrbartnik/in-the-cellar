<script setup lang="ts">
import BeersView from "@/views/BeersView.vue";
</script>

<template>
  <main>
    <BeersView :bottlesState="demoBeers" />
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
