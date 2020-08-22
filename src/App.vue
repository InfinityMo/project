<template>
  <div id="app">
    <router-view class="view-wrap" />
  </div>
</template>
<script>

export default {
  data () {
    return {

    }
  },
  computed: {

  },
  mounted () {

  },
  methods: {

  }
}
</script>
<style lang="less">
* {
  padding: 0;
  margin: 0;
}
body {
  transform: rotate(90deg);
  -ms-transform: rotate(90deg); /* Internet Explorer */
  -moz-transform: rotate(90deg); /* Firefox */
  -webkit-transform: rotate(90deg); /* Safari 和 Chrome */
  -o-transform: rotate(90deg); /* Opera */
  // background: #000;
}
#app {
  width: 100vh;
  height: 100vw;
  img {
    width: 100vh;
    height: 100vw;
  }
}
#app
// @media screen and (orientation: portrait)
{
  //   body {
  //     background: #fff;
  //   }
  //   #app .swiper-wrapper {
  //     width: 100%;
  //     height: 100vh;
  //     img {
  //       width: 100%;
  //       height: 100%;
  //     }
  //     .desaturate {
  //       filter: grayscale(100%);
  //       -webkit-filter: grayscale(100%);
  //       -moz-filter: grayscale(100%);
  //       -ms-filter: grayscale(100%);
  //       -o-filter: grayscale(100%);
  //     }
  //   }
  // }

  // /*横屏*/
  // @media screen and (orientation: landscape) {
  //   body {
  //     background: #fff;
  //   }
  //   #app .swiper-wrapper {
  //     width: 100%;
  //     height: 100vh;
  //     img {
  //       width: 100%;
  //       height: 100%;
  //     }
  //     .desaturate {
  //       filter: grayscale(100%);
  //       -webkit-filter: grayscale(100%);
  //       -moz-filter: grayscale(100%);
  //       -ms-filter: grayscale(100%);
  //       -o-filter: grayscale(100%);
  //     }
  //   }
}
</style>
