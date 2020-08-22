<template>
  <div class="page">
    <swiper :options="bannerOption">
      <swiper-slide v-for="(banner,index) in bannerList"
                    @click.native="changeDesaturate(index)"
                    :key="index"
                    class="banner-slide">
        <img :src="banner.url"
             :class="{'desaturate':banner.isdesaturate}">
      </swiper-slide>
    </swiper>
    <!-- <img src="../../../public/img/滨海大道.jpg"> -->
  </div>
</template>
<script>
import 'swiper/dist/css/swiper.css'
import { swiper, swiperSlide } from 'vue-awesome-swiper'
export default {
  name: 'Home',
  components: {
    swiper,
    swiperSlide
  },
  data () {
    return {
      bannerOption: {
        // direction: 'vertical',
        // pagination: {
        //   el: '.swiper-pagination',
        //   clickable: true
        // }
      },
      bannerList: [
        {
          isdesaturate: true,
          url: require('../../../public/img/滨海大道.jpg')
        },
        {
          isdesaturate: true,
          url: require('../../../public/img/滨海大道1985.jpg')
        },
        {
          isdesaturate: true,
          url: require('../../../public/img/盐田国际.jpg')
        },
        {
          isdesaturate: true,
          url: require('../../../public/img/福田中心区.jpg')
        }
      ]
    }
  },
  created () {

  },
  mounted () {

  },
  methods: {
    changeDesaturate (index) {
      this.bannerList[index].isdesaturate = false
    }
  }
}
</script>
<style lang="less" scoped>
</style>
