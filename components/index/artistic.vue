<template>
  <section class="m-istyle">
    <dl>
      <dt>有格调</dt>
      <dd class="all" @mouseenter="changeIn">全部</dd>
      <dd class="party" @mouseenter="changeIn">约会聚餐</dd>
      <dd class="spa" @mouseenter="changeIn">丽人SPA</dd>
    </dl>
    <ul class="ibody">
      <li v-if="item.type===hoverName || hoverName==='all'" v-for="(item,index) of allList" :key="index">
        <el-card>
          <img :src=item.content.img>
          <div class="cbody">
            <div class="title">{{item.content.name}}</div>
            <div class="desc">{{item.content.desc}}</div>
            <span class="price"><em>{{item.content.price}}</em></span>
            <span class="pos">{{item.content.pos}}</span>
          </div>
        </el-card>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  data () {
    return {
      hoverName: 'all',
      allList: [
        {
          type: 'party',
          content: {
            name: '金泉港IMAX国际影城',
            img: '//p0.meituan.net/poi/c2b482474377fc31a8311f46055f40b0442616.png@368w_208h_1e_1c',
            desc: '免押金,可停车,有情侣座,儿童票,有WIFI,IMAX厅,杜比全景声厅',
            price: '¥35.9',
            pos: '王府井/东单'
          }
        },
        {
          type: 'spa',
          content: {
            name: 'N&Franck 尼梵造型（东方广场店）',
            img: '//p1.meituan.net/merchantpic/fb7d33ada85c90dc398afd43280305ad47850.jpg@240w_180h_1e_1c_1l|watermark=1&&r=2&p=9&x=2&y=2&relative=1&o=20|368w_208h_1e_1c',
            desc: 'N&Franck 尼梵造型（东方广场店）',
            price: '¥241',
            pos: '王府井/东单'
          }
        },
        {
          type: 'spa',
          content: {
            name: 'うるおうき润熙美の研修社',
            img: '//p0.meituan.net/wedding/64d8fd076670a3b1d2a991f0262283ed625904.jpg@240w_180h_1e_1c_1l|watermark=1&&r=2&p=9&x=2&y=2&relative=1&o=20|368w_208h_1e_1c',
            desc: 'うるおうき润熙美の研修社',
            price: '',
            pos: '崇文门新世界'
          }
        },
        {
          type: 'party',
          content: {
            name: '天安瑞嘉烤鸭',
            img: '//p0.meituan.net/merchantpic/8d40aacd77004b484151c1ee547918d287691.jpg@368w_208h_1e_1c',
            desc: '烤鸭6人套餐，提供免费WiFi',
            price: '¥398',
            pos: '王府井/东单'
          }
        }
      ]
    }
  },
  methods: {
    changeIn (e) {
      let name = e.target.className
      this.hoverName = name
    }
  }
}
</script>

<style>

</style>
