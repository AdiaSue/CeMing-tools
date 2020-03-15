<template>
    <div class="box">
      <header class="mint-header is-fixed titleBox">
        <div class="is-left" @click="pageGoBack"></div>
        <div class="mint-header-title">行政区划</div>
        <div class="is-right"></div>
      </header>
      <div class="content division">
        <div class="searchArea">
          <div class="topSearch">
            <input type="text"  placeholder="请输入关键字查询" class="inputSearch" />
            <img src="@/assets/static/img/mob/searchClose.png" alt="" class="close"/>
            <span class="searchBtn">搜索</span>
          </div>
          <div class="serachList active">
            <div>重庆</div>
          </div>
        </div>
        <div class="hotCity list">
          <span>热门城市</span>
          <ul>
            <li>北京</li>
            <li>北京</li>
            <li>北京</li>
            <li>北京</li>
            <li>北京</li>
            <li>北京</li>
            <li>北京</li>
            <li>北京</li>
          </ul>
        </div>
        <div class="hotProvince list">
          <span>热门省份</span>
          <ul>
            <li>江苏</li>
            <li>江苏</li>
            <li>江苏</li>
            <li>江苏</li>
            <li>江苏</li>
            <li>江苏</li>
            <li>江苏</li>
            <li>江苏</li>
            <li>江苏</li>
          </ul>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'AdRegion',
  methods: {
    pageGoBack(){
      if(window.history.length <= 1){
        this.$router.push({ path: '/' });
        return false;
      } else {
        this.$router.go(-1);
      }
    }
  }
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

.topSearch{position: relative;}
.topSearch::before{
  position: absolute;
  left: .4rem;
  top: .15rem;
  content: "";
  display: inline-block;
  width: .44rem;
  height: .44rem;
  background: url(./../assets/static/img/mob/searchIcon.png) no-repeat;
  background-size: .44rem .44rem;
}
.topSearch .inputSearch{
  display: block;
  width: 6.14rem;
  height: .72rem;
  text-indent: .68rem;
  background-color:#f1f1f1;
  border-radius: .08rem;
  margin-left: .24rem;
  font-size: .26rem;
}
.topSearch>img.close{display: block;position: absolute;right: 1.3rem;top: .15rem;width: .44rem;height: .44rem;}
.topSearch>span.searchBtn{
  position: absolute;
  right: .24rem;
  color: #478eee;
  top: .15rem;
  font-size: .32rem;
  font-weight: 700;
}

.serachList{display: block;}
.serachList>div{padding: 0 .24rem;height: .8rem;line-height: .8rem;font-size: .24rem;color: #333;border-bottom: 1px solid #ddd;}
.active{display: block;}

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
</style>
