<template>
  <Svgicon
    :iconName="svgInfo.iconName"
    :width="svgInfo.width"
    :height="svgInfo.height"
    :color="svgInfo.color"
  ></Svgicon>
  <el-button @click="changeSvg">点我换图</el-button>
</template>
<script setup lang="ts">
import Svgicon from '@/components/Svgicon.vue'
import { ref } from 'vue'
let svgInfo = ref({
  iconName: 'home',
  width: '100px',
  height: '100px',
  color: 'red',
})

function changeSvg() {
  svgInfo.value.iconName = 'collapse'
  svgInfo.value.color = 'blue'
}
</script>
<style scoped lang="scss"></style>
