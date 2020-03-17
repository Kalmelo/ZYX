<template>
  <div class='tab'>
     这里是排行组件
     <mt-button type="default">default</mt-button>
      <mt-button type="primary">primary</mt-button>
      <mt-button type="danger">danger</mt-button>
      <hr>
      <h3>轮播图</h3>
      <mt-swipe  class='swier'>
        <mt-swipe-item class='test'>
          <img src="http://imgsrc.baidu.com/forum/w%3D580/sign=5a51a65e74ec54e741ec1a1689399bfd/3b6f91fa43166d2234243ef4492309f79152d290.jpg" alt="">
        </mt-swipe-item>
         <mt-swipe-item class='test'>
          <img src="http://imgsrc.baidu.com/forum/w%3D580/sign=fd16bc14a2345982c58ae59a3cf5310b/156029d062d9f2d33de70c8fa6ec8a136227cc75.jpg" alt="">
        </mt-swipe-item>
         <mt-swipe-item class='test'>
          <img src="http://imgsrc.baidu.com/forum/w%3D580/sign=3609b4bc8513632715edc23ba18ea056/f9bff70635fae6cd5c5f830100b30f2443a70f7f.jpg" alt="">
        </mt-swipe-item>
      </mt-swipe>
  </div>
</template>
<style lang="less" scoped>
@import '../../style/index.less';
.swier{
  height: 300px;
  .w(375);
  background: white;
  .test{
    .w(375);
    height: 350px;
    img{
      width: 100%;
      height: 100%;
    }
  }
}
</style>