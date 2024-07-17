<template>
  <svg :style="{ width, height }" :full="color">
    <use :href="prefix + iconName"></use>
  </svg>
</template>

<script setup lang="ts">
defineProps({
  prefix: {
    type: String,
    default: '#icon-',
  },
  iconName: {
    type: String,
    default: '',
  },
  width: {
    type: String,
    default: '16px',
  },
  height: {
    type: String,
    default: '16px',
  },
  color: {
    type: String,
    default: 'yellow',
  },
})
</script>

<style lang="scss" scoped></style>
