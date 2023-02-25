<template>
  <swiper
    :slidesPerView="3"
    :spaceBetween="30"
    :pagination="{
      clickable: true,
    }"
    :options="swiperOption"
    :modules="modules"
    class="mySwiper"
  >
    <swiper-slide><img src="../../assets/slider-1.png" alt="slider-1" /></swiper-slide>
    <swiper-slide><img src="../../assets/slider-2.png" alt="slider-1" /></swiper-slide>
    <swiper-slide><img src="../../assets/slider-3.png" alt="slider-1" /></swiper-slide>
    <swiper-slide><img src="../../assets/slider-3.png" alt="slider-1" /></swiper-slide>
  </swiper>
</template>
<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Pagination } from "swiper";
import "swiper/css";
import "swiper/swiper-bundle.min.css";

import "swiper/css/pagination";
const breakpoints = {
  640: {
    slidesPerView: 2,
    spaceBetween: 20,
  },
  768: {
    slidesPerView: 4,
    spaceBetween: 40,
  },
  1024: {
    slidesPerView: 5,
    spaceBetween: 50,
  },
};
export default {
  name: "slidervue",
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      modules: [Pagination],
      swiperOption: {
        slidesPerView: 7,
        spaceBetween: 30,
        loop: true,
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
      },
    };
  },
};
</script>
