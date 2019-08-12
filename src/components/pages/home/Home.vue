<template>
  <div>
    <home-header></home-header>
    <home-swiper></home-swiper>
  </div>
</template>

<script>
import HomeHeader from '@/components/pages/home/Header.vue'
import HomeSwiper from '@/components/pages/home/Swiper.vue'
export default {
  name: 'Home.vue',
  components: {
    HomeHeader,
    HomeSwiper
  }
}
</script>

<style scoped>

</style>
