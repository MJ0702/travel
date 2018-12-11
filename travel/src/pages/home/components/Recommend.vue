<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl">
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [
        {
          id: '0001',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1701/58/5873367611d51fa3.water.jpg_200x200_d86f0f19.jpg',
          title: '神仙居',
          desc: '融险峰、幽谷、秀林、奇瀑于一体'
        },
        {
          id: '0002',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1412/51/7022c84e0aa8987e63f0745a49c93161.water.jpg_200x200_27fdb337.jpg',
          title: '台州府城文化旅游区（江南长城）',
          desc: '融险峰、幽谷、秀林、奇瀑于一体'
        },
        {
          id: '0003',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/201405/13/cc6b2870049aa5086badad72fed0d36d.jpg_200x200_85a759dc.jpg',
          title: '天台山琼台仙谷',
          desc: '融险峰、幽谷、秀林、奇瀑于一体'
        },
        {
          id: '0004',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/201402/17/35d471cc22aea62ae922c08fa7477844.jpg_200x200_acae492c.jpg',
          title: '仙居',
          desc: '融险峰、幽谷、秀林、奇瀑于一体'
        },
        {
          id: '0005',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/201305/28/f06abca4216435a3c8d65eac.jpg_200x200_5e96deb2.jpg',
          title: '滑泥乐园',
          desc: '融险峰、幽谷、秀林、奇瀑于一体'
        },
        {
          id: '0006',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/201301/15/25172857c17b606a93835fbb.jpg_200x200_8fa6f7b0.jpg',
          title: '黄岩大瀑布',
          desc: '融险峰、幽谷、秀林、奇瀑于一体'
        },
        {
          id: '0007',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/201305/28/e2612882c26e7e09c8d65eac.jpg_200x200_c71d8d8c.jpg',
          title: '海盗村',
          desc: '融险峰、幽谷、秀林、奇瀑于一体'
        },
        {
          id: '0008',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1701/58/5873367611d51fa3.water.jpg_200x200_d86f0f19.jpg',
          title: '北洋蓝美庄园',
          desc: '融险峰、幽谷、秀林、奇瀑于一体'
        },
        {
          id: '0009',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/201406/06/a44369bc74c861237cdc6446ae322949.jpg_200x200_4feba072.jpg',
          title: '大鹿岛',
          desc: '融险峰、幽谷、秀林、奇瀑于一体'
        },
        {
          id: '0010',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/201301/16/fc71dce5dd55159293835fbb.jpg_200x200_28d0d581.jpg',
          title: '长屿硐天熊猫馆',
          desc: '融险峰、幽谷、秀林、奇瀑于一体'
        }
      ]
    }
  }
}
</script>
<style lang="stylus" scoped>
  @import '~styles/mixins.styl';
  .title
    margin-top:.2rem
    line-height:.8rem
    background:#eee
    text-indent:.2rem
  .item
    overflow:hidden
    display:flex
    height:1.9rem
    .item-img
      width:1.7rem
      height:1.7rem
      padding:.1rem
    .item-info
      flex:1
      padding:.1rem
      min-width:0
      .item-title
        line-height:.54rem
        font-size:.32rem
        ellipsis()
      .item-desc
        line-height:.4rem
        color:#ccc
        ellipsis()
      .item-button
        line-height:.44rem
        margin-top:.16rem
        background:#ff9300
        padding:0 .1rem
        border-radius:.06rem
        color:#fff
</style>
