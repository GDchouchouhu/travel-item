<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item in swiperlist " :key='item.id'>
        <img class="swiper-img" :src='item.imgsrc' alt="">
      </swiper-slide>

      <!-- Optional controls -->
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>
<script>
export default {
  name: 'HomeSwiper',
  data() {
    return {
      swiperOption: {
        pagination: '.swiper-pagination', //有小圆点
        loop: true //可循环
      },
      swiperlist: [
        {
          id: 1,
          imgsrc: 'https://gw.alicdn.com/imgextra/i1/78/O1CN01yeQtC91CRlPPiexoL_!!78-0-lubanu.jpg'
        },
        {
          id: 2,
          imgsrc: 'https://img.alicdn.com/imgextra/i2/67/O1CN01NiiRMD1CMj3I17yFc_!!67-0-luban.jpg'
        },
        {
          id: 3,
          imgsrc: 'https://gw.alicdn.com/imgextra/i4/31/O1CN01994Qh81C6EnGxQFIn_!!31-0-lubanu.jpg'
        }
      ]
    }
  }
}
</script>
<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active {
  background-color: #fff;
}

.wrapper {
  overflow: hidden;
  width: 100%;
  height: 0;
  padding-bottom: 31.25%;
  border-color: #eee;

  .swiper-img {
    width: 100%;
  }
}
</style>