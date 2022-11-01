<template>
  <button @click="$emit('click')">+</button>
</template>

<script lang="ts">
export default {
  name: "IncreaseButton",
};
</script>
