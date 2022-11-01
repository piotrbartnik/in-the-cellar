<template>
  <button>{{ message }}</button>
</template>

<script lang="ts">
export default {
  name: "IncreaseButton",
  props: { message: String },
};
</script>
