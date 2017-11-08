<template>
  <div class="index-part">
      <div class="notice-box">
        <div class="center">
          <p class="notice">
            <span class="tips">最新公告</span>
            <a class="info" :href="notice.url">{{notice.info}}</a>
          </p>
        </div>
      </div>
      <div class="part-box">
        <ul class="part-ul clearfix">
          <li class="part-li" v-for="(part,index) in parts" v-bind:key="index">
            <img class="part-pic" v-bind:src="part.pic" alt="">
            <p class="part-info">{{part.info}}</p>
          </li>
        </ul>
      </div>
  </div>
</template>

<script>


export default {
  name: 'IndexPart',
  data () {
    return {
      notice:{
        info: '[公告]欣荣钱包1.0今日起正式上线啦~',
        url: 'javascript:;'
      },
      parts: [{
        pic: './static/images/index/part1.png',
        info: '借款800以下，无需等待，极速放贷解您燃眉之急'
      },{
        pic: './static/images/index/part2.png',
        info: '绝不透露用户信息，保证用户信息安全'
      },{
        pic: './static/images/index/part3.png',
        info: '认证过程步骤简单、条理清晰，节省您的宝贵时间'
      },{
        pic: './static/images/index/part4.png',
        info: '暂时还不上？没关系！轻松展期一步到位'
      }]
    }
  }
}
</script>

<style lang="less" scoped>
  /*正文内容样式*/
  a:hover{
    color: #42beb6;
  }
  .notice-box{
    width: 100%;
    height: 50px;
    background-color: #fafafa;
    .center{
      width: 1200px;
      height: 50px;
      margin: 0 auto;
      .notice{
        line-height: 50px;
        color: #333;
        font-size: 14px;
        .tips{
          padding: 0 15px;
        }
      }
    }
  }
  /*模块样式*/
  .part-box{
    width: 100%;
    height: 400px;
    background: #FFF;
    .part-ul{
      width: 1100px;
      height: 100%;
      margin: 0 auto;
      .part-li{
        width: 25%;
        float: left;
        padding-top: 70px;
        text-align: center;
        .part-info{
          margin-top: 22px;
          width: 225px;
          display: inline-block;
          font-size: 14px;
          color: #999;
          text-align: left;
          letter-spacing: 1px;
        }
      }
    }
  }
</style>
