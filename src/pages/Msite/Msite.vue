<template>
  <div class="msite-container">

    <div class="HeaderTop">
      <span class="iconfont icon-sousuo search"></span>
     <p class="title" style="color: white; ">{{ title }}</p>
     <span class="user"><a href="javascript:;" style="color: white;">登录</a><span style="margin-left: 3px;margin-right: 3px; color: white;" >|</span><a href="javascript" style="color: white;">注册</a></span>
    
      <!-- 轮播图 -->
  <!-- Swiper -->
  <div class="imgs">
  <div class="swiper mySwiper">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <ul>
       <li><img class="imgList" src="../../common/images/nav/1.jpg" alt=""> <div>菜单1</div></li>
       <li><img class="imgList" src="../../common/images/nav/2.jpg" alt=""> <div>菜单1</div></li>
       <li><img class="imgList" src="../../common/images/nav/3.jpg" alt=""> <div>菜单1</div></li>
       <li><img class="imgList" src="../../common/images/nav/4.jpg" alt=""> <div>菜单1</div></li>
       <li><img class="imgList" src="../../common/images/nav/5.jpg" alt=""> <div>菜单1</div></li>
       <li><img class="imgList" src="../../common/images/nav/6.jpg" alt=""> <div>菜单1</div></li>
       <li><img class="imgList" src="../../common/images/nav/7.jpg" alt=""> <div>菜单1</div></li>
       <li><img class="imgList" src="../../common/images/nav/8.jpg" alt=""> <div>菜单1</div></li>
        </ul>
        </div>


        <div class="swiper-slide">
          <ul>
       <li><img class="imgList" src="../../common/images/nav/9.jpg" alt=""> <div>外卖2</div></li>
       <li><img class="imgList" src="../../common/images/nav/10.jpg" alt=""> <div>外卖2</div></li>
       <li><img class="imgList" src="../../common/images/nav/11.jpg" alt=""> <div>外卖2</div></li>
       <li><img class="imgList" src="../../common/images/nav/12.jpg" alt=""> <div>外卖2</div></li>
       <li><img class="imgList" src="../../common/images/nav/13.jpg" alt=""> <div>外卖2</div></li>
       <li><img class="imgList" src="../../common/images/nav/14.jpg" alt=""> <div>外卖2</div></li>
       <li><img class="imgList" src="../../common/images/nav/1.jpg" alt=""> <div>外卖2</div></li>
       <li><img class="imgList" src="../../common/images/nav/2.jpg" alt=""> <div>外卖2</div></li>
        </ul>
        </div>
   
      </div>
        </div>
           <!--分页器 -->
           <div class="swiper-pagination"></div>
      </div>
    <!-- 商家选择栏 -->
    <div class="shop_header">
      <span>三</span>
      <span>附近商家</span>
      <ShopList>
        <template #img>
          <img src="../../images/shop/1.jpg" alt="">
        </template>
        <template #title>
  锄禾日当午，汗滴禾下土
        </template>
      </ShopList>
      
      <ShopList>
        <template #img>
          <img src="../../images/shop/2.jpg" alt="">
        </template>
        <template #title>
  床前明月光疑似地上霜
        </template>
      </ShopList>
      <ShopList>
        <template #img>
          <img src="../../images/shop/3.jpg" alt="">
        </template>
        <template #title>
  举头望明月低头思故乡
        </template>
      </ShopList>
      <ShopList>
        <template #img>
          <img src="../../images/shop/4.jpg" alt="">
        </template>
        <template #title>
  假如生活欺骗了你不要
        </template>
      </ShopList>
  
  
      <!-- ../../images/shop/1.jpg -->
      
   
    </div>
    </div>



      </div>
    
    

 </template>

<script>

import Swiper from "swiper";
import ShopList from '../../components/ShopList/ShopList.vue'
// import style (<= Swiper 5.x) 6.0以下版本的样式引入方法
import 'swiper/css/swiper.css'


export default {
  data(){
      return {
        title:'主页标题地址',
        url1:"../../images/shop/1.jpg"
      }
    },
    components:{
      Swiper,ShopList
    },
    mounted(){
      // 轮播图的使用
      var swiper = new Swiper(".mySwiper", {
        pagination: {
          el: ".swiper-pagination",
       
        },
    
      }); 
// ================================轮播图结束位置
    }
   
}
</script>

<style scoped>
*{
  padding: 0;
  margin: 0;
}
a{
  color: black;
  text-decoration: none;
}
li{
  font-style: normal;
  list-style: none;
}
.msite-container{
  background: #4c00ff;
}
.HeaderTop{

  position: fixed;
        left: 0;
        top: 0;
        width :100%;
        height: 45px;
      
        background-color: #02a774;
}
.title{
position: absolute;
left: 50%;

transform: translateX(-50%);
margin-top: 15px;
/* 
text-align: center; */
}
.user{
  
    position: absolute;
    right: 20px;
  bottom: 10px;
  
}
.search{
  position: absolute;
    left: 20px;
  bottom: 10px;
  color: white;
}

/* 轮播图设置 */
.swiper-slide{
  height: 200px;
  width: 390px;
}
.imgs{
  position: fixed;
  top: 45px;
  height: 230px;
  background-color: white;
}
.imgs ul{
  width: 390px;
  height: 100%;
}


.imgs  li{
  float: left;

margin: 20px 20px 20px 25px;
}
.imgList div{
  text-align: center;
 
}
.imgList{
  width: 50px;
  height: 50px;
}
/* 分页器设置 */
.swiper-pagination{
  position: absolute;
  left: 185px;

  bottom: 5px;
}
/* 商家选择栏区 */
.shop_header{
 
  color: #999;
  position: fixed;
  top: 35%;
  width: 100%;
  height: 20px;
  padding: 10px 10px 0px 10px;
  background-color: white;
  line-height: 20px;
}
.shop_header span{
  margin-left: 3px;
}
/* 商家栏 */

/* iconfont矢量图图标样式设置 */
@font-face {
  font-family: "iconfont"; /* Project id 4056924 */
  src: url('//at.alicdn.com/t/c/font_4056924_l8dv7t95az.woff2?t=1683596956341') format('woff2'),
       url('//at.alicdn.com/t/c/font_4056924_l8dv7t95az.woff?t=1683596956341') format('woff'),
       url('//at.alicdn.com/t/c/font_4056924_l8dv7t95az.ttf?t=1683596956341') format('truetype');
}

.iconfont {
  font-family: "iconfont" !important;
  font-size: 18px;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
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