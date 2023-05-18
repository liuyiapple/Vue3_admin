<template>
  <div>
    <svg :style="{ width, height }">
      <use :xlink:href="`#icon-${name}`" :fill="color"></use>
    </svg>
  </div>
</template>
<script lang="ts" setup>
defineProps({
  name: {
    type: String,
    default: '',
  },
  color: {
    type: String,
    default: '',
  },
  width: {
    type: String,
    default: '30px',
  },
  height: {
    type: String,
    default: '30px',
  },
})
</script>
<style lang="less" scoped></style>
