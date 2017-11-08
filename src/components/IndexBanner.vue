<template>
  <div class="index-banner">
    <div class="banner">
      <div class="center">
        <div class="qrcode-box">
          <img class="qr-pic" :src="qrcode" alt="">
          <p class="qr-tips">扫码关注微信公众号</p>
        </div>
        <div class="act-box">
          <img class="act-pic" :src="phone" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>


export default {
  name: 'IndexBanner',
  data () {
    return {
      qrcode: './static/images/index/qrcode.png',
      phone: './static/images/index/phone.png'
    }
  }
}
</script>

<style lang="less" scoped>
  /*中间banner样式*/
.index-banner{
  width: 100%;
  height: 628px;
  .banner{
    overflow: hidden;
    width: 100%;
    height: 100%;
    background: url("../assets/banner.jpg") no-repeat center;
    background-size: cover;
    .center{
      position: relative;
      width: 1200px;
      height: 100%;
      margin: 0 auto;
      .qrcode-box{
        position: absolute;
        left: 12px;
        bottom: 65px;
        .qr-pic{
          display:block;
        }
        .qr-tips{
          margin-top: 30px;
          padding-left: 2px;
          color: #FFF;
          line-height: 30px;
          font-size: 21px;
          letter-spacing: 1px;
        }
      }
      .act-pic{
        position: absolute;
        right: -32px;
        top: 105px;
      }
    }
  }
}

</style>
