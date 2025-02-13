<script setup></script>

<template>
  <div class="ly-header">
    <div class="title">
      <div class="logo"></div>
      <div class="name">DC - SDK</div>
    </div>
    <div class="menus"></div>
  </div>
</template>

<style lang="scss" scoped>
.ly-header {
  position: fixed;
  z-index: 999;
  width: 100%;
  height: 60px;
  background: #2c2c2c;
  color: #fff;
  display: flex;
  .title {
    width: 200px;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    .name {
      font-weight: bold;
    }
  }
}
</style>
