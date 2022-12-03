<template>
  <span>{{ beerName }}</span>
  <ActionButton @click="decrement" message="-" decreaseButton />
  <ActionButton @click="increment" message="+" />
  <span>{{ amountOfBottles }} </span>
</template>

<script lang="ts">
import ActionButton from "./ActionButton.vue";

export default {
  data() {
    return {
      msg: "Counter App",
      amountOfBottles: this.$props.initialAmount,
    };
  },
  props: {
    beerName: String,
    initialAmount: {
      type: Number,
      required: true,
    },
  },
  methods: {
    increment() {
      this.amountOfBottles += 1;
    },

    decrement() {
      if (this.initialAmount) {
        this.amountOfBottles -= 1;
      }
    },
  },
  components: { ActionButton },
};
</script>
