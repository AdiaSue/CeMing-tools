<template>
    <div class="cm clear">
      <img class="bg" src="@/assets/static/img/mob/moblieBG.png" alt="小微律政智能公司测名系统"/>
      <section class="form">
        <div class="item">
          <span class="title">行政区域</span>
          <router-link to="/AdRegion">北京</router-link>
        </div>
        <div class="item">
          <span class="title">企业字号</span>
          <input class="mint-field-core" type="text" placeholder='请输入企业字号，如"XXXX"'/>
        </div>
        <div class="item">
          <span class="title">行业分类</span>
          <a href="javascript:;">北京</a>
        </div>
        <div class="item">
          <span class="title">组织类型</span>
          <a href="javascript:;">北京</a>
        </div>
        <button type="button">公司测名</button>
      </section>
      <section class="record">
        <header>公司测名记录<a href="javascript:;">更多 ></a></header>
        <a class="clear" href="javascript:;">
          <span>哈尔滨毅美润科技有限公司</span>
          <span class="time">13秒前</span>
        </a>
        <a class="clear" href="javascript:;">
          <span>哈尔滨毅美润科技有限公司</span>
          <span class="time">13秒前</span>
        </a>
        <a class="clear" href="javascript:;">
          <span>哈尔滨毅美润科技有限公司</span>
          <span class="time">13秒前</span>
        </a>
        <a class="clear" href="javascript:;">
          <span>哈尔滨毅美润科技有限公司</span>
          <span class="time">13秒前</span>
        </a>
        <a class="clear" href="javascript:;">
          <span>哈尔滨毅美润科技有限公司</span>
          <span class="time">13秒前</span>
        </a>
        <a class="clear" href="javascript:;">
          <span>哈尔滨毅美润科技有限公司</span>
          <span class="time">13秒前</span>
        </a>
      </section>
      <footer><a href="javascript:;">XXXX官网 ></a></footer>
    </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home'
}
</script>

<style scoped>
.cm{background-color: #f2f3f4;}
.cm>img.bg{width: 100%;position: absolute;top: 0;}

.form{
  width: 94%;
  position: relative;
  z-index: 1;
  background-color: #ffffff;
  box-shadow: 0.02rem 0 0.14rem 0 rgba(0,0,0,.2);
  border-radius: .2rem;
  margin: 62% auto 0;
  padding: .24rem .4rem 1.04rem;
}
.form .item{
  display: flex;
  height: .92rem;
  line-height: .92rem;
  border-radius: .08rem;
  border: .02rem solid #ddd;
  position: relative;
  margin: 0 auto;
  margin-top: .56rem;
}
.form .item .title{-webkit-box-flex: 0;flex: none;color: #666;padding: .28rem .24rem 0 .33rem;font-size: .28rem;line-height: .38rem;}
.form .item span+a{-webkit-box-flex: 1;flex: 1;position: relative;color: #333;font-size: 13px;}
.form .item span+a:after{
  border-color: #666;
  border-style: solid;
  border-width: .03rem .03rem 0 0;
  content: " ";
  top: 50%;
  right: .32rem;
  position: absolute;
  width: .18rem;
  height: .18rem;
  -webkit-transform: translateY(-50%) rotate(45deg);
  -ms-transform: translateY(-50%) rotate(45deg);
  transform: translateY(-50%) rotate(45deg);
}
.mint-field-core{width: 100%;}
.form button{
  height: .92rem;
  width: 97%;
  text-align: center;
  background: #1972ea;
  border-radius: .08rem;
  margin: 0 auto;
  margin-top: .96rem;
  color: #fff;
  position: relative;
  font-weight: 700;
}

.record{padding: .64rem;}
.record>header{font-size: .32rem;color:#333;line-height: .44rem;font-weight: 700;padding-bottom: .08rem;}
.record>header>a{color: #1972ea;font-size: .28rem;float: right;font-weight: 400;margin-top:-.02rem;}
.record>a{display: block;margin-top: .32rem;}
.record>a>span{display: inline-block;}
.record>a>span:first-child{
  color: #333;
  font-size: .3rem;
  line-height: .38rem;
  max-width: 79%;
  overflow: hidden;
  -o-text-overflow: ellipsis;
  text-overflow: ellipsis;
  white-space: nowrap;
  float: left;
}
.record>a>span.time{
  color: #999;
  font-size: .24rem;
  float: right;
  line-height: .38rem;
}

footer{text-align: center;padding: .16rem 0 .62rem;}
footer>a{color: #1972ea;font-size: .28rem;line-height: .38rem;}
</style>
