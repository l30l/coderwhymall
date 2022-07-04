<template>
  <div class="tab-bar-item" @click="itemClick">
    <div class="active-icon" v-if="isActive">
      <slot name="active-icon"></slot>
    </div>
    <div class="item-icon" v-else>
      <slot name="item-icon"></slot>
    </div>
    <div class="item-text" :class="{ active: isActive }">
      <slot name="item-text"></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TabBarItem',
  data() {
    return {}
  },
  methods: {
    itemClick() {
      this.$router.push(this.path)
      console.log(this.$route.path)
      console.log(this.path)
    }
  },
  props: {
    path: String
  },
  computed: {
    isActive() {
      return this.$route.path.indexOf(this.path) !== -1
      // 为什么第一遍按4个按钮都是false，但是功能却没问题呢
    }
  }
}
</script>

<style scoped>
.tab-bar-item {
  flex: 1;
  padding: 4px 0;
  text-align: center;
}
.tab-bar-item img {
  width: 24px;
  vertical-align: middle;
}
.tab-bar-item span {
  font-size: 14px;
}
.active {
  color: #c33979;
}
</style>
