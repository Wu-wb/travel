<template>
    <div class="swiper">
      <swiper :options="swiperOption" >
        <swiper-slide v-for="(item,index) in swiperList" :key="item.id">
          <img class="swiper-img" :src="item.imUrl" />
        </swiper-slide>
        <!-- Optional controls -->
        <div class="swiper-pagination"  slot="pagination"></div>
      </swiper>
    </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true // 支持循环轮播
      },
      swiperList: [{
        id: '001',
        imUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20198/ffb06b600df4c655d10a1dfef4a8d0e9.jpg_750x200_7b1aec5e.jpg'
      }, {
        id: '002',
        imUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20198/da3db1d9761f8984fd9c84c4eccf93ee.jpg_750x200_b7f8686a.jpg'
      }, {
        id: '003',
        imUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20196/01549e224da474a72681614810d07860.jpg_750x200_47325a53.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .swiper >>>.swiper-pagination-bullet-active
    background:#fff !important
  .swiper
    overflow:hidden
    width:100%
    height: 0
    padding-bottom: 26.666%
    background-color:#eee
    .swiper-img
      width :100%
</style>
