<template>
    <div class="box">
      <header class="mint-header is-fixed titleBox">
        <div class="is-left"></div>
        <div class="mint-header-title">组织类型</div>
        <div class="is-right"></div>
      </header>
      <div class="content division">
        <div class="list">
          <span>内资企业</span>
          <ul>
            <li>有限公司</li>
            <li>股份有限公司</li>
            <li>股份公司</li>
            <li>合伙企业</li>
            <li>中心</li>
            <li>事务所</li>
            <li>经营部</li>
            <li>店</li>
            <li>商行</li>
            <li>厂</li>
            <li>工作室</li>
          </ul>
        </div>
        <div class="list">
          <span>外资企业</span>
          <ul>
            <li>有限责任公司</li>
            <li>有限公司</li>
            <li>股份有限公司</li>
            <li>股份公司</li>
            <li>合伙企业</li>
            <li>中心</li>
            <li>事务所</li>
            <li>工作室</li>
            <li>商行</li>
          </ul>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'TypeOfOrgan'
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
.list>ul{padding-top: .24rem;padding-left: 2.6%;overflow: hidden;}
.list>ul>li{
  float: left;
  width: 31%;
  height: 10%;
  font-size: .28rem;
  line-height: .84rem;
  text-align: center;
  box-shadow: 0.04rem 0 0.24rem 0 rgba(3,14,30,.2);
  border-radius: .04rem;
  margin-right: 2%;
  margin-bottom: 2%;
}
.list>ul>li:nth-child(3n){margin-right:0;}
</style>
