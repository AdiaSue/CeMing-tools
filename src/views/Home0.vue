<template>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <header>
      <div class="headerInner clear">
        <div :class="[{'leftNav':true},{'BJSeleted':mainLocatIsClick}]">
          <div class="mainLoc" @click="switchMainLocalClass">
            <img src="@/assets/static/img/location.svg"/>
            <span class="light">北京站</span>
            <i class="selArrow"></i>
          </div>
          <div class="hotCity">
            <div class="title">
              <span>热门城市</span>
              <a href="javascript:;">更多城市<i></i></a>
            </div>
            <div class="list">
              <a href="javascript:;" v-for="(city,i) in hotCityList" :key="i">{{city}}</a>
            </div>
          </div>
        </div>
        <div class="rightNav">
          <a href="javascript:;">登录</a>
          <a href="javascript:;">注册</a>
          <a href="javascript:;">我的订单</a>
          <a href="javascript:;">个人中心</a>
          <a href="javascript:;"><img src="@/assets/static/img/iphone.svg"/>联系我们</a>
        </div>
      </div>
    </header>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  data () {
    return {
      mainLocatIsClick: false,
      hotCityList: ['北京', '上海', '天津', '广州', '深圳', '杭州', '长沙', '济南', '西安', '沈阳']
    }
  },
  components: {
    // HelloWorld
  },
  methods: {
    switchMainLocalClass () {
      this.mainLocatIsClick = !this.mainLocatIsClick
    }
  }
}
</script>

<style scoped>
header{width: 100%;position: fixed;top: 0;left: 0;z-index: 100;background: #fff;}
header img{width: 18px;vertical-align: middle;}
.headerInner{width:1200px;margin:0 auto;border:0px solid red;}
.leftNav{width: 360px;height: 40px;float: left;margin-left: 29px;position: relative;}
.mainLoc{
  display: inline-block;
  height: 40px;
  position: relative;
  z-index: 200;
  line-height: 40px;
  color: #333;
  background: #fff;
  border: 1px solid rgba(0,0,0,0);
  border-bottom: 0;
  border-top: 0;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  padding-right: 10px;
  font-size: 0;
}
.mainLoc>img{width: 18px;vertical-align: middle;margin-left: 10px}
.mainLoc>span.light{vertical-align: middle;display: inline-block;margin: 0 8px;font-size: 12px;}
.mainLoc>i.selArrow{
  display: inline-block;
  width: 16px;
  height: 16px;
  position: relative;
  top: 7px;
  cursor: pointer;
  background: url(./../assets/static/img/locDown.png) no-repeat 50%;
}
.hotCity{
  position: absolute;
  top: 39px;
  left: 0;
  z-index: 150;
  display: none;
  padding: 20px 30px;
  width: 360px;
  background: #fff;
  border: 1px solid #eee;
}
.hotCity .title{overflow: hidden;margin-bottom: 20px;line-height: 24px;}
.hotCity .title>span{float: left;color: #333;font-weight: 700;}
.hotCity .title>a{float: right;font-style: normal;font-size: 12px;color: #1972ea;}
.hotCity .title>a>i{
  display: inline-block;
  width: 16px;
  height: 16px;
  vertical-align: middle;
  margin-top: -4px;
  background: url(./../assets/static/img/locRight.png) no-repeat 50%;
}
.hotCity .list{overflow: hidden;}
.hotCity .list>a{
  width: 48px;
  height: 24px;
  line-height: 24px;
  text-align: center;
  font-size: 12px;
  color: #333;
  margin-right: 14px;
  margin-bottom: 5px;
  font-weight: 700;
  float: left;
}
.hotCity .list>a:nth-child(5n){margin-right: 0;}
.hotCity .list>a:hover{background: #1972ea;border-radius: 2px;color: #fff;}

.rightNav{float: right;padding-right: 30px;}
.rightNav>a{display: inline-block;line-height: 40px;font-size: 12px;color: #333;margin-left: 44px;}
.rightNav>a>img{margin-right: 8px;}

.BJSeleted .mainLoc{border: 1px solid #eee;border-bottom: 0;border-top: 0;color: #1972ea;}
.BJSeleted .hotCity{display: block;}
.BJSeleted i.selArrow{background: url(./../assets/static/img/locUp.png) no-repeat 50%;}
</style>
