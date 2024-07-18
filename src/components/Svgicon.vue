<template>
  <svg :style="{ width, height }">
    <use :href="prefix + iconName" :fill="color"></use>
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
