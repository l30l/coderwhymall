<template>
  <div>
    <nav-bar>
      <span slot="center">购物街</span>
    </nav-bar>
  </div>
</template>

<script>
import NavBar from '@/components/common/navBar/NavBar.vue'
export default {
  components: { NavBar },
  name: 'HomeNavBar'
}
</script>

<style scoped>
span {
  color: #fff;
}
</style>
