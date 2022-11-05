<template>
  <ActionButton @click="decrement" message="-" decreaseButton />
  <ActionButton @click="increment" message="+" />
  <span>{{ value }} </span>
</template>

<script lang="ts">
import ActionButton from "./ActionButton.vue";

export default {
  data() {
    return {
      msg: "Counter App",
      value: 0,
    };
  },
  methods: {
    increment() {
      this.value += 1;
    },

    decrement() {
      if (this.value) {
        this.value -= 1;
      }
    },
  },
  components: { ActionButton },
};
</script>
