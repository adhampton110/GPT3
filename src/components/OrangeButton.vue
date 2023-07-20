<script setup>
defineProps({
  message: String,
  borderRadius: String,
  width: Number,
  height: Number,
})

const cssProps = computed ( () => {
  return {
    '--borderRadius': this.borderRadius,
    '--width': this.width,
    '--height': this.height,
  }
})
</script>

<template>
  <button>{{ message }}</button>
</template>

<style scoped>
button {
  border-radius: var(--borderRadius);
  width: var(--width);
  height: var(--height);
}
</style>
