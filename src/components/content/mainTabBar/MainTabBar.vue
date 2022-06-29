<template>
  <div class="main-tab-bar">
    <tab-bar>
      <tab-bar-item path="/home">
        <img slot="active-icon" src="@/assets/img/tabbar/home-active.svg" alt="" />
        <img slot="item-icon" src="@/assets/img/tabbar/home.svg" alt="" />
        <span slot="item-text">Home</span>
      </tab-bar-item>
      <tab-bar-item path="/category">
        <img slot="active-icon" src="@/assets/img/tabbar/category-active.svg" alt="" />
        <img slot="item-icon" src="@/assets/img/tabbar/category.svg" alt="" />
        <span slot="item-text">Category</span>
      </tab-bar-item>
      <tab-bar-item path="/cart">
        <img slot="active-icon" src="@/assets/img/tabbar/cart-active.svg" alt="" />
        <img slot="item-icon" src="@/assets/img/tabbar/cart.svg" alt="" />
        <span slot="item-text">Cart</span>
      </tab-bar-item>
      <tab-bar-item path="/profile">
        <img slot="active-icon" src="@/assets/img/tabbar/profile-active.svg" alt="" />
        <img slot="item-icon" src="@/assets/img/tabbar/profile.svg" alt="" />
        <span slot="item-text">Profile</span>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
import { TabBar, TabBarItem } from '@/components/common/tabBar'

export default {
  name: 'MainTabBar',
  components: {
    TabBar,
    TabBarItem
  },
  methods: {}
}
</script>

<style scoped></style>
