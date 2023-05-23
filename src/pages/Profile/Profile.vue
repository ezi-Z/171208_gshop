<template>
    <div>
     <h2> Profile</h2>
     <div class="HeaderTop">
     <p class="title">{{ title }}</p>
     <router-link to="/login">
      <div class="ProfileTop">
        <!-- 头像 -->
        <div class="topLeft"><img src="../../common/images/nav/7.jpg" alt=""></div>
        <span class="topRight">
         <span style="font-size: 20px;"> 登录/注册</span>
         
         <div style="margin-top: -15px;font-size: 14px;"> <span class="iconfont icon-shoujihao"></span> 暂无手机绑定号</div>
        </span>
        <span class="iconfont icon-xiangyoujiantou jt"></span>
      </div>
     </router-link>


     <!-- 会员剩余余额 -->
     <div class="balacnce">
      <div class="box" style="color: rgb(39, 215, 148);">
           0.00  <span>元</span>
          <p>我的余额</p>

      </div>

      <div class="box" style="color: rgb(44, 173, 233);">
           0.00  <span>个</span>
          <p>我的优惠</p>

      </div>


           <div class="box" style="color: rgb(233, 139, 15);">
           0.00  <span>分</span>
          <p>我的积分</p>

      </div>


      <div class="bottom" style="margin-top: 0px;">
        <a href="javascript:;" style="margin-left: 10px;">
          <span class="iconfont icon-dingdan1" style="color:#02a774;"></span>
          <span class="ht">
            我的订单
          </span>
          <span class="iconfont icon-xiangyoujiantou" style="margin-left: 250px; font-size: 16px;"></span>
        </a>
        
      </div>

      <div class="bottom">
        <a href="javascript:;" style="margin-left: 10px;">
          <span class="iconfont icon-jifen" style="color:#ff5f3e;"></span>
          <span class="ht">
            积分商城
          </span>
          <span class="iconfont icon-xiangyoujiantou" style="margin-left: 250px; font-size: 16px;"></span>
        </a>
        
      </div>

      <div class="bottom">
        <a href="javascript:;" style="margin-left: 10px;">
          <span class="iconfont icon-huiyuanqiaguanli" style="color:#f90;"></span>
          <span class="ht">
            硅谷外卖会员卡
          </span>
          <span class="iconfont icon-xiangyoujiantou" style="margin-left: px; font-size: 16px;"></span>
        </a>
        
      </div>

      <div class="bottom" style="margin-top: 15px;">
        <a href="javascript:;" style="margin-left: 10px;">
          <span class="iconfont icon-a-3yewufuwuzhongxin" style="color:#02a774;"></span>
          <span class="ht">
            服务中心
          </span>
          <span class="iconfont icon-xiangyoujiantou" style="margin-left: 250px; font-size: 16px;"></span>
        </a>
        
      </div>

      
     </div>

    </div>
    </div>
  </template>
  
  <script>
  export default {
    data(){
      return {

        title:'我的'
      }
    },
    components:{
    },
  }
  </script>
  

  <style scoped>
*{
  margin: 0;
  padding: 0;
}
.HeaderTop{
  color: white;
  position: fixed;
        left: 0;
        top: 0;
        width :100%;
        height: 45px;
        background-color: #02a774;
        /* border-bottom: 3px solid white; */
        line-height: 45px;
    
}

a{
  color: black;
  text-decoration: none;
}
.topRight{
  margin-left: 20px;
  /* margin-bottom: 10px; */
  margin-top: -5px;
  color: white;
  float: left;
  
}
.topRight::before{
  contain: '>';
}
.title{
/* position: absolute;
left: 50%;
transform: translateX(-50%); */

text-align: center;
}
.ProfileTop{

  width: 100%;
  height: 60px;
  padding: 20px 10px 20px 10px;
  background-color: #02a774;
  margin-top: 1px;
}

/* 头像 */
.topLeft{
  float: left;
  display: inline-block;
  width: 68px;
  height: 68px;
  overflow: hidden;
  border-radius: 50%;
}
.jt{
  margin-top: 10;
  color: white;
  float: right;
  margin-right: 20px;
}
/*  会员信息 */
.balacnce{
    width: 100%;
   background-color: white;
    height: 82px;
}
/* 会员信息的小盒子 */
.balacnce .box{
  display: inline-block;
  width: 33%;
  height: 100%;
  margin-left: 1px;
  overflow: hidden;
  text-align: center;
  line-height: 60px;
  font-size: 30px;
  color: coral;
}
.box span{
  font-size: 16px;
  color: rgb(0, 0, 0);
}
.box p{
  z-index: 9999;
  color: black;
  font-size: 14px;
  margin-top: -30px;
}


/* 最下面链接区域 */
.bottom{
  background-color: white;
}
.ht{
font-size: 18px;

}
@font-face {
  font-family: "iconfont"; /* Project id 4056924 */
  src: url('//at.alicdn.com/t/c/font_4056924_4cw0l0rrucq.woff2?t=1684563870294') format('woff2'),
       url('//at.alicdn.com/t/c/font_4056924_4cw0l0rrucq.woff?t=1684563870294') format('woff'),
       url('//at.alicdn.com/t/c/font_4056924_4cw0l0rrucq.ttf?t=1684563870294') format('truetype');
}

.iconfont {
  font-family: "iconfont" !important;
  font-size: 20px;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  vertical-align:bottom;
}

.icon-jifen:before {
  content: "\e898";
}

.icon-huiyuanqiaguanli:before {
  content: "\e63a";
}

.icon-dingdan1:before {
  content: "\e98d";
}

.icon-a-3yewufuwuzhongxin:before {
  content: "\e65b";
}
.icon-xiangyoujiantou:before {
  content: "\e65f";
}

.icon-shoujihao:before {
  content: "\e62b";
}

.icon-pingfen_xuanzhong:before {
  content: "\e877";
}

.icon-shuyi_xing-pingfen:before {
  content: "\e668";
}

.icon-sousuo:before {
  content: "\e62f";
}

.icon-wode:before {
  content: "\e600";
}

.icon-dingdan:before {
  content: "\e897";
}

.icon-waimai-:before {
  content: "\e606";
}

</style>