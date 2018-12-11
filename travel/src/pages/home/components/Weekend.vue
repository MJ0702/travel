<template>
  <div>
    <div class="title">周末推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of weekendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl">
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      weekendList: [
        {
          id: '0001',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1811/15/66f14e0fd6fbb.jpg_r_640x214_5d69f21d.jpg',
          title: '南国冰雪乐园',
          desc: '这里可以让你在南国感受到北国风光'
        },
        {
          id: '0002',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1811/f8/29dfa785277839.jpg_r_640x214_7d051523.jpg',
          title: '阳江温泉知多少',
          desc: '这里的天空和大海让人心旷神怡，配上舒缓的优美音乐，泡个暖暖的温泉岂不美哉'
        },
        {
          id: '0003',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1811/b8/5d599bbdcf8b57.jpg_r_640x214_2ee055e3.jpg',
          title: '浮在海上的绿洲',
          desc: '南国滨海之城，避寒胜地，有暖暖的阳光，海风习习，吃着海鲜逛逛老街多惬意啊'
        },
        {
          id: '0004',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1505/b9/f9d8ace21c06.jpg_r_640x214_1f239a81.jpg',
          title: '粤东泡汤好去处',
          desc: '全时四季的温泉，度假的天堂'
        },
        {
          id: '0005',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1505/fa/ca65fde9677de2.jpg_r_640x214_4500e3ff.jpg',
          title: '深圳必游TOP10',
          desc: '来到深圳，你需要来这里签到'
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
  .item-img-wrapper
    overflow:hidden
    height:0
    padding-bottom:33.9%
    .item-img
      width:100%
  .item-info
    padding:.1rem
    .item-title
      line-height:.54rem
      font-size:.32rem
      ellipsis()
    .item-desc
      line-height:.4rem
      ellipsis()
</style>
