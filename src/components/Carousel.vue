<template>
  <swiper ref="mySwiper" :options="swiperOptions">
    <swiper-slide :key="image" v-for="image in images">
      
    </swiper-slide>
    
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
</template>

<script>
  export default {
    data() {
      return {
        images: [
            '../assets/img/Dickhead.PNG',
            '../assets/img/gnomesmile.PNG',
        ],
        swiperOptions: {
          pagination: {
            el: '.swiper-pagination'
          },
          loop:true,
          slidesPerView: 1,
          centeredSlides: true,
          initialSlide: 0,
          autoplay: {
              disableOnInteraction: true
          },
          direction: "horizontal",
          // Some Swiper option/callback...
        }
      }
    },
    computed: {
      swiper() {
        return this.$refs.mySwiper.$swiper
      }
    },
    mounted() {
    // //   console.log('Current Swiper instance object', this.swiper)
    //   console.log(this.swiper.slides.length);
    //   this.swiper.slideTo(1, 1000, true)
    //   setTimeout(() => {
    //       this.swiper.slideTo(1, 1000, true)

    //   }, 1000)

    
      
    },
    methods: {
    }
  }
</script>