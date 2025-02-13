<script setup>
import LyHeader from './layout/LyHeader.vue'
import LyContent from './layout/LyContent.vue'
</script>

<template>
  <div class="container">
    <ly-header></ly-header>
    <ly-content></ly-content>
  </div>
</template>

<style lang="scss" scoped>
.container {
  width: 100%;
  height: 100%;
  user-select: none;
}
</style>
