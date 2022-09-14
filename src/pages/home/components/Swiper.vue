<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl" />
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: "HomeSwiper",
  data() {
    return {
      swiperOption: {
        pagination: ".swiper-pagination",
        loop: true,
      },
      swiperList: [
        {
          id: "0001",
          imgUrl:
            "https://tr-osdcp.qunarzz.com/tr-osd-vs-dapp-ugc/img/be049a68a045fa43ecc1044e5bbbd343.jpg",
        },
        {
          id: "0002",
          imgUrl:
            "https://tr-osdcp.qunarzz.com/tr-osd-vs-dapp-ugc/img/441e13aef8edd94ebe4e1c665bf1f62e.jpg",
        },
      ],
    };
  },
};
</script>

<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active {
  background: fff !important;
}

.wrapper {
  overflow: hidden;
  width: 100%;
  padding-bottom: 180;
  background: #000;

  .swiper-img {
    width: 100%;
  }
}
</style>