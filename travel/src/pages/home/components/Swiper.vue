<template>
    <div class="wrapper">
      <swiper :options="swiperOption">
        <!-- slides -->
        <swiper-slide v-for="item of swiperList" :key="item.id">
          <img class="swiper-img" :src="item.imgUrl">
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
        loop: true
      },
      swiperList: [
        {
          id: '0001',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1812/e0/7aed5dde53dabe02.jpg_750x200_9b7a65fd.jpg'
        },
        {
          id: '0002',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/b7/1e9c4ca462741f02.jpg_750x200_842d5261.jpg'
        },
        {
          id: '0003',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1811/a8/cb43c4ac6c215d02.jpg_750x200_83dee994.jpg'
        },
        {
          id: '0004',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1802/d1/af067e81b43fe02.jpg_750x200_d2499d48.jpg'
        }
      ]
    }
  }
}
</script>
<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background:#FFF
  .wrapper
    overflow:hidden
    width:100%
    height:0
    padding-bottom:26.7%
    background:#eee
    .swiper-img
      width :100%
</style>
