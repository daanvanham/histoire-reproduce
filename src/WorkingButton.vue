<template>
  <button :class="`--${color}`"><slot /></button>
</template>

<script lang="ts">
// Vendor
import { defineComponent } from "vue";

export default defineComponent({
  props: {
    color: {
      type: String,
      default: "primary",
    },
  },
});
</script>

<style lang="scss">
// just a comment here
</style>

<style lang="scss" scoped>
.--primary {
  background-color: var(--color-primary);
}
</style>
