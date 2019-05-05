<template>
  <div class="slider">
    <el-row :gutter="10" class="up">
      <el-col :span="14">
        <el-carousel class="big">
          <el-carousel-item v-for="item in 4" :key="item">
            <h3 class="small">{{ item }}</h3>
          </el-carousel-item>
        </el-carousel>
      </el-col>
      <el-col :span="4">
        <a href="#">
          <div class="life"></div>
        </a>
      </el-col>
      <el-col :span="6">
        <div class="login-wrap">
          <div class="img-wrap">
            <img class="img" src="//s0.meituan.net/bs/fe-web-meituan/2d05c2b/img/avatar.jpg" alt="">
          </div>
          <p class="desc">Hi！你好</p>
          <div>
            <el-button round class="login">注册</el-button>
          </div>
          <div>
            <el-button round class="register">立即登录</el-button>
          </div>
        </div>
      </el-col>
    </el-row>
    <el-row :gutter="10" class="under">
      <el-col :span="7">
        <a href="#">
          <div class="hotel"></div>
        </a>
      </el-col>
      <el-col :span="7">
        <a href="#">
          <div class="posture"></div>
        </a>
      </el-col>
      <el-col :span="4">
        <a href="#">
          <div class="seller"></div>
        </a>
      </el-col>
      <el-col :span="6">
        <div class="mt-wrap">
          <div class="img-wrap">
            <img class="img" src="//s1.meituan.net/bs/fe-web-meituan/60ac9a0/img/download-qr.png" alt="">
          </div>
          <p class="desc">美团APP手机版</p>
          <div class="desc2">
            <span class="price">1元起</span><span class="play">吃喝玩乐</span>
          </div>
        </div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'slider'
}
</script>

<style lang="stylus" scoped>
  .slider
    .up
      padding: 10px 0 10px 13px
      .big
        height: 240px
      .life
        height: 240px
        background-image: url('http://p0.meituan.net/codeman/e473bb428f070321269b23370ff02ba956209.jpg')
        background-size: 100% 100%
      .login-wrap
        box-sizing: border-box;
        text-align: center
        padding-top: 30px
        height: 240px
        background-color: #fff
        border: 1px solid #eee
        .img
          width: 55px
          height: 55px
          border-radius: 50%
        .desc
          padding: 5px 0
          font-size: 16px
        .login, .register
          width: 120px
        .login
          margin-bottom: 15px
    .under
      padding: 0 0 10px 13px
      .hotel
        height: 165px
        background-image: url('http://p1.meituan.net/codeman/8cce56c467a17e04f3094d1e455462a0132772.png')
        background-size: 100% 100%
      .posture
        height: 165px
        background-image: url('http://p1.meituan.net/codeman/16442c19da1f1c4544f794e29d99c92051716.jpg')
        background-size: 100% 100%
      .seller
        height: 165px
        background-image: url('http://p1.meituan.net/codeman/5b21cddb4bb1cbc3a9c3bce0f726c75940469.jpg')
        background-size: 100% 100%
      .mt-wrap
        box-sizing: border-box;
        text-align: center
        padding-top: 10px
        height: 165px
        background-color: #fff
        border: 1px solid #eee
        .img-wrap
          .img
            width: 95px
            height: 95px
        .desc
          font-size: 16px
        .desc2
          .play, .price
            font-size 12px
          .price
            color: #EC5330
            margin-right: 4px
</style>
