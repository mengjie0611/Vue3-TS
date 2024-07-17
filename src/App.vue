<template>
  <!-- <el-button type="primary">按钮</el-button> -->
  <Svgicon iconName="home" width="100px" height="100px" color="red"></Svgicon>
</template>
<script setup lang="ts">
import zhCn from 'element-plus/dist/locale/zh-cn.mjs'
import { ref } from 'vue'
import Svgicon from '@/components/Svgicon.vue'

const locale = ref(zhCn)
console.log(locale.value)
</script>
<style scoped lang="scss"></style>
