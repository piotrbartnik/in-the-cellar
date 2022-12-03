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
  align-items: center;
  justify-content: center;
  position: relative;
  box-sizing: border-box;
  cursor: pointer;
  font-weight: 500;
  font-size: 0.875rem;
  line-height: 1.75;
  text-transform: uppercase;
  min-width: 64px;
  padding: 5px 15px;
  border-radius: 4px;
  border: 1px solid #00000070;
  color: #000000;
  display: inline-flex;
}

.decrease {
  background-color: #e92b2bd0;
}

.increase {
  background-color: #60c960c0;
}
</style>
