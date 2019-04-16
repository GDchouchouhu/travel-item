<template>
  <div>
    <div class='recom-title'>热销推荐</div>
    <ul>
      <li>
        <div class="item border-bottom" v-for="item in itemlist" :key="item.id">
          <img class='item-img' :src="item.imgsrc" alt="">
          <div class="item-info">
            <p class="item-title">{{item.title}}</p>
            <p class="item-desc">{{item.desc}}</p>
            <button class="item-button">查看详情</button>
          </div>
        </div>
      </li>
    </ul>

  </div>
</template>
<script>
export default {
  name: 'HomeRecommend',
  data() {
    return {
      itemlist: [
        {
          id: 1,
          imgsrc:
            'https://img.alicdn.com/bao/uploaded///gw.alicdn.com/imgextra/TB1_NkPXcbpK1RjSZFySut_qFXa.jpg_230x230.jpg',
          title: '美丽巴厘岛欢迎你们到，赶快来吧扫努奥。实打实的的阿达',
          desc: '巴厘岛是印度尼西亚很美丽的岛屿，所以要用 flex:1 和min-width: 0弄不要超出;'
        },
        {
          id: 2,
          imgsrc:
            'https://img.alicdn.com/bao/uploaded///gw.alicdn.com/imgextra/TB1_NkPXcbpK1RjSZFySut_qFXa.jpg_230x230.jpg',
          title: '美丽巴厘岛欢迎你们到，赶快来吧扫努奥。实打实的的阿达',
          desc: '巴厘岛是印度尼西亚很美丽的岛屿，所以要用 flex:1 和min-width: 0弄不要超出;'
        },
        {
          id: 3,
          imgsrc:
            'https://img.alicdn.com/bao/uploaded///gw.alicdn.com/imgextra/TB1_NkPXcbpK1RjSZFySut_qFXa.jpg_230x230.jpg',
          title: '美丽巴厘岛欢迎你们到，赶快来吧扫努奥。实打实的的阿达',
          desc: '巴厘岛是印度尼西亚很美丽的岛屿，所以要用 flex:1 和min-width: 0弄不要超出;'
        }
      ]
    }
  }
}
</script>
<style lang="stylus" scoped>
@import '~styles/overmin.styl';

.recom-title {
  margin-top: 0.2rem;
  line-height: 0.8rem;
  background-color: #eeeeee;
  text-indent: 0.2rem;
}

.item {
  overflow: hidden;
  display: flex;
  height: 1.9rem;
  margin-left: 0.2rem;

  .item-img {
    width: 2.1rem;
    height: 1.7rem;
    padding: 0.1rem;
  }

  .item-info {
    flex: 1;
    margin-left: 0.2rem;
    padding: 0.1rem;
    min-width: 0;

    .item-title {
      line-height: 0.54rem;
      font-size: 0.32rem;
      overminfun();
    }

    .item-desc {
      line-height: 0.4rem;
      color: #ccc;
      overminfun();
    }

    .item-button {
      line-height: 0.44rem;
      margin-top: 0.16rem;
      background: #ff9300;
      padding: 0 0.2rem;
      border-radius: 0.06rem;
      color: #fff;
    }
  }
}
</style>
