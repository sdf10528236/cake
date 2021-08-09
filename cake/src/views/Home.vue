<template>
  <div>
    <swiper
      ><div class="swiper-slide">
        <img class="swiperimg01" src="../assets/home_swiper/img06.jpg" />
      </div>
      <div class="swiper-slide">
        <img class="swiperimg01" src="../assets/home_swiper/img07.jpg" />
      </div>
      <div class="swiper-slide">
        <img class="swiperimg01" src="../assets/home_swiper/img05.png" />
      </div>
    </swiper>
    <router-view />
  </div>
</template>

<script>
/* eslint-disable */

// Import Swiper styles
import swiper from "@/views/Home/Swiper";
export default {
  data() {
    return {
      datalist: [],
      imglist: [
        "../assets/home_swiper/img01.jpg",
        "@/assets/home_swiper/img02.jpg",
        "@/assets/home_swiper/img03.jpg",
      ],
    };
  },
  mounted() {
    setTimeout((this.datalist = [1, 2, 3]), 2000);
  },
  components: { swiper },
};
</script>
<style lang="scss" scoped>
.swiper-slide {
  width: 100%;
  overflow: hidden;
  height: 500px;

  .swiperimg01 {
    margin-top: -5%;
    width: 100%;
  }
}

@media (max-width: 950px) {
  .swiper-slide {
    height: auto;
    min-height: 337px;
  }
}

@media screen and (max-width: 760px) {
  .swiper-slide {
    height: auto;
    min-height: 270px;
  }
}
@media screen and (max-width: 585px) {
  .swiper-slide {
    height: auto;
    min-height: 202px;
  }
}
@media screen and (max-width: 380px) {
  .swiper-slide {
    height: auto;
    min-height: 135px;
  }
}
</style>