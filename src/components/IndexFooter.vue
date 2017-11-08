<template>
  <div class="index-footer">
    <div class="center">
      <div class="footer clearfix">
        <p class="info">
          <img class="icon" src="../assets/icon_phone.png" alt="">
          <span class="text">0574-87769600</span>
        </p>
        <p class="info">
          <img class="icon" src="../assets/icon_wx.png" alt="">
          <span class="text">欣荣钱包</span>
        </p>
        <p class="info">
          <img class="icon" src="../assets/icon_email.png" alt="">
          <span class="text">xrqb@xrjinrong.com</span>
        </p>
        <p class="info">
          <img class="icon" src="../assets/icon_home.png" alt="">
          <span class="text">深圳市前海深港合作区前湾一路1号A栋201室</span>
        </p>
      </div>
      <div class="copyright">
        <p class="info">Copyright © 深圳欣荣金融信息服务有限公司 粤ICP备17079605号-1</p>
      </div>
    </div>
  </div>
</template>

<script>


export default {
  name: 'IndexFooter',
  data () {
    return {

    }
  }
}
</script>

<style lang="less" scoped>
  .index-footer{
    width: 100%;
    background-color: #222729;
    .center{
      width:800px;
      height: 100%;
      margin: 0 auto;
      .partner{
        width: 100%;
        height: 220px;
        border-bottom: 1px solid #000;
        .tips{
          color: #ccc;
          font-size: 24px;
          padding-top: 30px;
        }
      }
      .footer{
        width: 100%;
        height: 62px;
        color: #5c6163;
        font-size: 14px;
        text-align: center;
        border-top: 1px solid #676767;
        border-bottom: 1px solid #000;
        .info{
          float: left;
          padding: 32px 16px 0;
        }
      }
      .copyright{
        width: 100%;
        height: 68px;
        border-top: 1px solid #676767;
        .info{
          text-align: center;
          line-height: 68px;
          font-size: 14px;
          color: #41484c;
        }
      }
    }
  }
</style>
