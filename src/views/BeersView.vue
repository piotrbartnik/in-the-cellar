<script setup lang="ts">
import BeerCounter from "@/components/BeerCounter.vue";
</script>

<template>
  <div class="beerContainer">
    <div
      v-for="value in bottlesState"
      v-bind:key="value.name"
      class="singleBeer"
    >
      <BeerCounter :beerName="value.name" :initialAmount="value.currentAmout" />
    </div>
  </div>
</template>

<style>
.beerContainer {
  display: flex;
  flex-wrap: nowrap;
  flex-direction: column;
  width: 100%;
}

.singleBeer {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 10px;
}
</style>

<script lang="ts">
export default {
  props: {
    bottlesState: Object,
  },
};
</script>
