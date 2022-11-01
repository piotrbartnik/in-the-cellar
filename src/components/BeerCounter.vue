<template>
  <button @click="decrement">-</button>
  <IncreaseButton @click="increment">+</IncreaseButton>
  <span>{{ value }} </span>
</template>

<script lang="ts">
import IncreaseButton from "./IncreaseButton.vue";

export default {
  data() {
    return {
      msg: "Counter App",
      value: 0,
    };
  },
  methods: {
    increment(test: string) {
      this.value += 1;
      console.log("clicked", test);
    },

    decrement() {
      this.value -= 1;
    },
  },
  components: { IncreaseButton },
};
</script>
