<template>
  <button
    class="actionButton"
    :class="{ decrease: decreaseButton, increase: !decreaseButton }"
  >
    {{ message }}
  </button>
</template>

<script lang="ts">
export default {
  name: "IncreaseButton",
  props: { message: String, decreaseButton: Boolean },
};
</script>

<style>
.actionButton {
  cursor: pointer;
}

.decrease {
  background-color: #ff0000;
}

.increase {
  background-color: #008000;
}
</style>
