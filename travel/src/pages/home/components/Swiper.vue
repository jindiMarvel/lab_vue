<template>
    <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide>
      <img class="swiper-img" src="https://img1.qunarzz.com/vc/af/f4/45/4756cd165e1462610598ceb201.png" />
      </swiper-slide>
      <swiper-slide>
      <img class="swiper-img" src="https://img1.qunarzz.com/vc/31/cc/75/3c014d49de263aea6bf9bffeda.png" />
      </swiper-slide>
      <swiper-slide>
      <img class="swiper-img" src="https://img1.qunarzz.com/vc/af/f4/45/4756cd165e1462610598ceb201.png" />
      </swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
      <div class="swiper-button-prev" slot="button-prev"></div>
      <div class="swiper-button-next" slot="button-next"></div>
      <div class="swiper-scrollbar"   slot="scrollbar"></div>
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
      }
    }
  }
}
</script>
<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background: #fff
  .wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 31.25%
    background: #eee
    .swiper-img
      width: 100%
</style>
