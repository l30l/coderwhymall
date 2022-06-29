<template>
  <div class="tab-bar">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'TabBar'
}
</script>

<style scoped>
.tab-bar {
  position: fixed;
  bottom: 0;
  display: flex;
  width: 100%;
  height: 49px;
  background: #f6f6f6;
}
</style>
