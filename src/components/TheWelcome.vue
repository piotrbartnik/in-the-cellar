<template>
  <button @click="decrement">-</button>
  <button @click="increment">+</button>
  <span>{{ value }} </span>
</template>

<script lang="ts">
export default {
  data() {
    return {
      msg: "Counter App",
      value: 0,
    };
  },
  methods: {
    decrement() {
      if (this.value) {
        this.value -= 1;
      }
    },
    increment() {
      this.value += 1;
    },
  },
};
</script>
