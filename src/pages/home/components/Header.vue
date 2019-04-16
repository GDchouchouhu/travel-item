<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>输入城市/景点/游玩主题</div>
    <div class="header-right">
      城市
      <span class="iconfont arrow-icon">&#xe64a;</span></div>

  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>
<style lang="stylus" scoped>
@import '~styles/varibles';

.header {
  display: flex;
  line-height: $headerHeight;
  background-color: $bgColor;
  color: #fff;
// 文件设置是50px,手机减半。本来是86 /2 /50 等于 86/100=0.86
  .header-left {
    width: 0.64rem;
    // width: 32px
    float: left;

    .back-icon {
      text-align: center;
      font-size: 0.4rem;
    }
  }

  .header-input {
    flex: 1;
    height: 0.64rem;
    background-color: #fff;
    line-height: 0.64rem;
    margin-top: 0.12rem;
    margin-left: 0.2rem;
    padding-left: 0.2rem;
    border-radius: 0.1rem;
    color: #ccc;
  }

  .header-right {
    min-width: 1.04rem;
    padding: 0 0.1rem;
    float: right;
    text-align: center;
    color: #fff;

    .arrow-icon {
      margin-left: -0.04rem;
      font-size: 0.24rem;
    }
  }
}
</style>


