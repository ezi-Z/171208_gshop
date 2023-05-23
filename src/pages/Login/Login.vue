<template>
  <div class="login-container">
    <span class="iconfont icon-fanhuijiantou return" @click="goTO"></span>
      <div class="loginInner">
        <h2>硅谷外卖</h2>
        <div class="select-dl">
        <router-link to="/left"  class="dxdl dl" :class="{on: isCurrent('/left')}">短信登录</router-link>
        <router-link to="/right" class="mmdl dl" :class="{on: isCurrent('/right')}">密码登录</router-link>
        </div>
        <!-- :class="{ on:isCount('/left')}" -->
        <router-view></router-view>
      </div>

  </div>
</template>

<script>
import Jquery from 'jquery';

export default {

  methods:{
    goTO(){
      this.$router.push('/profile')
    },
    isCurrent(path) {
// console.log(this.$route.path)
    return this.$route.path === path
    
} ,

}

}

</script>

<style scoped>
  *{
    padding: 0;
    margin: 0;
  }
  .mmdl{
    margin-bottom: 10px;
  }
  a{
    text-decoration: none;
    color: black;
  }
  
  /* 硅谷外卖标题 */
  h2{
    text-align: center;
    margin-left: -15px;
    font-size: 38px;
    color: #02a774;
  }
  /* 外部大盒子 */
  .loginInner{
    width: 321px;
    height: 380px;
    /* background-color: pink; */
    padding-top: 60px;
    margin-left: 40px;
    margin-right: 40px;
  }
  .on{
    padding-bottom: 2px;
    border-bottom: #23936f 1px solid;
    color: #23936f;
  }
  /* 登录选择按键 */
  .select-dl{
    text-align: center;
    margin-top: 40px;
    margin-left: 60px;
    display: inline-block;
 
    text-decoration: none;
  }
.dl{
  /* color: black; */
  /* text-decoration: none; */
  display: inline-block;
  margin-left: 15px;
}
/* 返回箭头设置 */

.return{
  position: fixed;
}


  @font-face {
  font-family: "iconfont"; /* Project id 4056924 */
  src: url('//at.alicdn.com/t/c/font_4056924_91htnpea9fq.woff2?t=1684306509156') format('woff2'),
       url('//at.alicdn.com/t/c/font_4056924_91htnpea9fq.woff?t=1684306509156') format('woff'),
       url('//at.alicdn.com/t/c/font_4056924_91htnpea9fq.ttf?t=1684306509156') format('truetype');
}
.iconfont {
  font-family: "iconfont" !important;
  font-size: 28px;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.icon-fanhuijiantou:before {
  content: "\e8b5";
}

</style>