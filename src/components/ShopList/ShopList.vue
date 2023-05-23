<template>
  <div class="shoplist-container">
    <a href="">
   
        <div class="shop-left">
            <!-- <img src="../../images/shop/1.jpg" alt=""> -->
         
          <slot name="img"></slot>
        </div>
        <div class="shop-right">
            <div class="top">
                <div class="pp">{{pp}}</div>
                <span class="title"> <slot name="title"></slot> </span>
                <span class="right_text">保  准  票</span>
         
            </div>
            <div class="mid">
                <div class="mid_left">
                    <span class="iconfont icon-pingfen_xuanzhong"></span>
                    <span class="iconfont icon-pingfen_xuanzhong"></span>
                    <span class="iconfont icon-pingfen_xuanzhong"></span>
                    <span class="iconfont icon-shuyi_xing-pingfen"></span>
                    <span class="iconfont icon-shuyi_xing-pingfen"></span>
                    <span class="mid_left_text">3.6</span>
                    
                    <span class="mid_right_text">
                        <span>硅谷传送</span>
                    </span>
                </div>
            </div>
            
            <div class="bottom">
                <span style="color:#999;font-size: 10px;">20起送/配送费约5</span>
            </div>
        </div>
        
    </a>
    
  </div>
</template>

<script>
export default {
  props:[
  
  ],
    data(){

        return{
            pp:"品牌",
            title:"锄禾日当午，汗滴禾下土",
        }
    },
    created(){
      console.log(this.url);
    }

}</script>

<style scoped>
a{
  color: black;
  text-decoration: none;
}
    .shoplist-container{
      position: relative;
        width: 100%;
        height: 75px;
        margin-top:-1px ;
        margin-left: -16px;
        padding: 18px 8px 15px 8px;
        background-color: white;
   
    }
    /* 商家图片 */
    .mid{
        margin-top: 10px;
        margin-bottom: 5px;
    }
    .shop-left{
        padding-right: 10px;

    }
    .shop-left img {
        width: 76px;
        height: 75px;
        margin-left: 5px;
    }
/* 右边结构 */
    .shop-right{
        position: absolute;
        width: 289px;
        height: 74px;
        background-color: white;
        bottom: 16px;
        right: 17px;
    }
    .pp{
        font-size: 3px;
        text-align: center;
        line-height: 11px;
        width: 24px;
        height: 11px;
        padding: 2px;
        margin-right: 5px;
        margin-top: 3px;
        background-color: #ffb300;
    }
    /* 标题 */
    .title{
       width: 100px;
        position: absolute;
        top: 0;
        left: 33px;
        font-size: 16px;

            /* 强制不换行 */
    white-space: nowrap;
    /* 匀速溢出内容，隐藏 */
    overflow: hidden;
    /* 文字用省略号代替超出的部分 */
    text-overflow: ellipsis;
    }
    .right_text{

        position: absolute;
        top: 0;
        right: 0px;
        font-size: 8px;
        color: #999;
  
    }
    .mid_left_text{
  
        color:#f5640b;
        font-size: 10px;
        margin-left: 2px;
    }
   .mid_right_text{
    margin-left: 160px;
    font-size: 12px;
    color: #02a774;
    border: solid 1px #02a774;
   }
    /* iconfont */
    @font-face {
  font-family: "iconfont"; /* Project id 4056924 */
  src: url('//at.alicdn.com/t/c/font_4056924_nhrwxkkipng.woff2?t=1684134999594') format('woff2'),
       url('//at.alicdn.com/t/c/font_4056924_nhrwxkkipng.woff?t=1684134999594') format('woff'),
       url('//at.alicdn.com/t/c/font_4056924_nhrwxkkipng.ttf?t=1684134999594') format('truetype');
}

.iconfont {
  font-family: "iconfont" !important;
  font-size: 12px;
    color:#ef8441;
 
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
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

