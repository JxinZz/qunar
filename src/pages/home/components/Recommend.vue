<template>
  <div>
    <div class="recommend-title">热销推荐</div>
    <ul>
      <li
        class="item border-bottom"
        v-for="item of recommendList"
        :key="item.id"
      >
        <img class="item-img" :src="item.imgUrl" />
        <div class="item-info">
          <p class="item-title">{{ item.title }}</p>
          <p class="item-desc">{{ item.desc }}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "HomeRecommend",
  data() {
    return {
      recommendList: [
        {
          id: "0001",
          imgUrl:
            "https://img1.qunarzz.com/sight/p0/2005/39/3979f1867defec4ea3.water.jpg_256x160_6ae804bb.jpg",
          title: "八达岭长城",
          desc: "不到长城非好汉",
        },
        {
          id: "0001",
          imgUrl:
            "https://img1.qunarzz.com/sight/p0/2005/39/3979f1867defec4ea3.water.jpg_256x160_6ae804bb.jpg",
          title: "八达岭长城",
          desc: "不到长城非好汉",
        },
        {
          id: "0001",
          imgUrl:
            "https://img1.qunarzz.com/sight/p0/2005/39/3979f1867defec4ea3.water.jpg_256x160_6ae804bb.jpg",
          title: "八达岭长城",
          desc: "不到长城非好汉",
        },
        {
          id: "0001",
          imgUrl:
            "https://img1.qunarzz.com/sight/p0/2005/39/3979f1867defec4ea3.water.jpg_256x160_6ae804bb.jpg",
          title: "八达岭长城",
          desc: "不到长城非好汉",
        },
        {
          id: "0001",
          imgUrl:
            "https://img1.qunarzz.com/sight/p0/2005/39/3979f1867defec4ea3.water.jpg_256x160_6ae804bb.jpg",
          title: "八达岭长城",
          desc: "不到长城非好汉",
        },
      ],
    };
  },
};
</script>

<style lang="stylus" scoped>
@import '~@/assets/styles/mixins.styl';

.recommend-title {
  line-height: 0.8rem;
  background: #eee;
  text-indent: 0.2rem;
}

.item {
  overflow: hidden;
  display: flex;
  height: 1.9rem;

  .item-img {
    width: 1.7rem;
    height: 1.7rem;
    padding: 0.1rem;
  }

  .item-info {
    flex: 1;
    padding: 0.1rem;
    min-width: 0;

    .item-title {
      line-height: 0.54rem;
      font-size: 0.32rem;
      ellipsis();
    }

    .item-desc {
      line-height: 0.4rem;
      color: #ccc;
      ellipsis();
    }

    .item-button {
      line-height: 0.44rem;
      margin-top: 0.16rem;
      background: #ff9300;
      padding: 0 0.2rem;
      border-radius: 0.6rem;
      color: #fff;
    }
  }
}
</style>