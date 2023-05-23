<template>
  <div class="footguide-container">

    <!-- <routr-link to="/msite">外卖</routr-link>
    <routr-link to="/search">搜索</routr-link>
    <routr-link to="/order">订单</routr-link>
    <routr-link to="/profile">我的</routr-link> -->
    <div class="box">
     <a href="#/msite">
        <!-- :class="{on: isCurrent('/msite')}" -->
        <div class="iconfont icon-waimai-"></div>
        <div class="guide">外卖</div>
     </a>
    </div>
    <div class="box">
     <a href="#/search">
        <div class="iconfont icon-sousuo"></div>
        <div class="guide">搜索</div>
     </a>
    </div>
    <div class="box">
     <a href="#/order">
        <div class="iconfont icon-dingdan"></div>
        <div class="guide">订单</div>
     </a>
    </div>
    <div class="box">
     <a href="#/profile">
        <div class="iconfont icon-wode"></div>
        <div class="guide">我的</div>
     </a>
    </div>
  
  </div>
</template>

<script>
 import $ from "jquery";

export default {

    methods:{
  

    }
   

}
</script>

<style scoped>
a{
    color: black;
    text-decoration: dashed;
}
*{
    margin: 0;
    padding: 0;
}
.footguide-container{
  
    position: fixed;
    background-color: #02a774;
    width: 100%;
    height: 50px;
    bottom: 0;
    left: 0;
    border-top: 1px solid rgb(209, 201, 201);
}

.box{
    display: inline-block;
    width: 25%;
    text-align: center;
    margin-top: 3px;
}
/* 设置高亮部分 */
.box .on{

    color: blue;
}


/* iconfont矢量图图标样式设置 */
@font-face {
  font-family: "iconfont"; /* Project id 4056924 */
  src: url('//at.alicdn.com/t/c/font_4056924_l8dv7t95az.woff2?t=1683596956341') format('woff2'),
       url('//at.alicdn.com/t/c/font_4056924_l8dv7t95az.woff?t=1683596956341') format('woff'),
       url('//at.alicdn.com/t/c/font_4056924_l8dv7t95az.ttf?t=1683596956341') format('truetype');
}

.iconfont {
  font-family: "iconfont" !important;
  font-size: 24px;
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

