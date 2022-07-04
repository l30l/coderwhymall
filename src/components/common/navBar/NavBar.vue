<template>
  <div class="nav-bar">
    <div class="left">
      <slot name="left"></slot>
    </div>
    <div class="center">
      <slot name="center"></slot>
    </div>
    <div class="right">
      <slot name="right"></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style scoped>
.nav-bar {
  display: flex;
  width: 100%;
  height: 44px;
  background: var(--color-tint);
  line-height: 44px;
  text-align: center;
}
.left,
.center,
.right {
  flex: 1;
}
</style>
