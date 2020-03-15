<template>
    <div class="box">
      <header class="mint-header is-fixed titleBox">
        <div class="is-left"></div>
        <div class="mint-header-title">行业分类</div>
        <div class="is-right"></div>
      </header>
      <div class="content division">
        <div class="blueTag">
          <img src="@/assets/static/img/mob/markIcon.png" alt="" />
          <span>提交您的商标查询需求，我们将为您提供查询服务。</span>
          <img src="@/assets/static/img/mob/searchClose.png" alt="" />
        </div>
        <div class="list">
          <span>科技类</span>
          <ul>
            <li>科技</li>
            <li>网络科技</li>
            <li>电子商务</li>
            <li>电子科技</li>
            <li>环保科技</li>
            <li>生物科技</li>
            <li>教育科技</li>
            <li>信息技术</li>
          </ul>
        </div>
        <div class="list">
          <span>许可类</span>
          <ul>
            <li>投资管理</li>
            <li>资产管理</li>
            <li>融资租赁</li>
            <li>医疗器械</li>
            <li>人力资源</li>
            <li>劳务派遣</li>
            <li>食品</li>
            <li>金融</li>
          </ul>
        </div>
        <div class="list">
          <span>服务类</span>
          <ul>
            <li>广告</li>
            <li>文化传播</li>
            <li>文化发展</li>
            <li>文化传媒</li>
            <li>建筑装潢</li>
            <li>建筑设计</li>
            <li>信息咨询</li>
            <li>教育咨询</li>
            <li>投资咨询</li>
            <li>管理咨询</li>
            <li>培训</li>
            <li>美容美发</li>
            <li>房地产经纪</li>
            <li>物业管理</li>
            <li>商业咨询</li>
            <li>企业管理</li>
            <li>餐饮管理</li>
            <li>家政服务</li>
          </ul>
        </div>
        <div class="list">
          <span>其他</span>
          <ul>
            <li>贸易</li>
            <li>商贸</li>
            <li>实业</li>
            <li>制造</li>
            <li>服饰</li>
            <li>化妆品</li>
            <li>工程</li>
            <li>农业</li>
            <li>建筑工程</li>
          </ul>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'ClassOfIndus'
}
</script>

<style scoped>
.box{background-color: #ffffff;min-height: 100vh;max-height:100vh;overflow: auto;width:100%;padding-top: .9rem;}
.mint-header{
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  background-color: #26a2ff;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  color: #fff;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  font-size: 14px;
  height: 40px;
  line-height: 1;
  padding: 0 10px;
  position: relative;
  text-align: center;
  white-space: nowrap;
}
.mint-header.is-fixed{top: 0;right: 0;left: 0;position: fixed;}
.titleBox{width: 100%;height: .88rem;background-color: #fff;padding: 0 .2rem;}
.titleBox .is-left{height: .44rem;position: relative;}
.titleBox .is-left:after{
  content: "";
  position: absolute;
  left: .1rem;
  top: .1rem;
  height: .19rem;
  width: .19rem;
  border-top: .04rem solid #000;
  border-left: .04rem solid #000;
  -webkit-transform: rotate(-45deg);
  -ms-transform: rotate(-45deg);
  transform: rotate(-45deg);
}
.titleBox .mint-header-title{color: #333;font-weight: 600;font-size: .36rem;-webkit-box-flex: 0;flex: none;margin: 0 auto;}

.list>span{color: #333;font-size: .32rem;font-weight: 700;display: block;padding: .48rem .24rem .24rem;border-bottom: 1px solid #ddd;}
.list>ul{padding-top: .24rem;padding-left: 1.9%;overflow: hidden;}
.list>ul>li{
  float: left;
  width: 23%;
  height: 10%;
  font-size: .28rem;
  line-height: .84rem;
  text-align: center;
  box-shadow: 0.04rem 0 0.24rem 0 rgba(3,14,30,.2);
  border-radius: .04rem;
  margin-right: 2%;
  margin-bottom: 2%;
}
.list>ul>li:nth-child(4n){margin-right:0;}
.blueTag{padding: .4rem .24rem;overflow: hidden;line-height: .33rem;background-color: #1972ea;display: flex;align-items: center;justify-content: space-between;}
.blueTag>img{width: .36rem;height: .36rem;display: block;}
.blueTag>span{color: #fff;font-size: .24rem;font-weight: 700;display: block;padding-left: 3%;}
</style>
