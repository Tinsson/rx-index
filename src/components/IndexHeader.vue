<template>
  <div class="index-header">
    <div class="center clearfix">
      <div class="logo-box">
        <img class="main-logo" src="../assets/logo.png" alt="">
        <img class="sub-logo" src="../assets/logo2.png" alt="">
      </div>
      <div class="user-box">
        <a href="javascript:;" class="user-opt">下载APP</a>
        <a href="javascript:;" class="user-opt">关注我们</a>
        <span class="user-opt line">|</span>
        <a href="javascript:;" class="user-opt">客服</a>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'IndexHeader',
  data () {
    return {

    }
  }
}
</script>

<style lang="less" scoped>
  /*公用部分样式*/
  a:hover{
    color: #42beb6;
  }
  #inblk{
    display: inline-block;
  }
  /*头部样式*/
  .index-header{
    width: 100%;
    height: 81px;
    background-color: #FFF;
    .center{
      width: 1200px;
      margin: 0 auto;
      .logo-box{
        float: left;
        .main-logo{
          #inblk;
          margin: 20px 0 0 8px;
        }
        .sub-logo{
          #inblk;
          margin: 23px 0 0 35px;
        }
      }
      .user-box{
        float: right;
        font-size: 17px;
        margin-top: 30px;
        .user-opt{
          margin: 0 4px;
          &.line{
            vertical-align: top;
          }
        }
      }
    }
  }

</style>
