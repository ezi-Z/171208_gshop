<template>
  <div>
    <!-- <h1>短信登录</h1> -->
    <div class="top">
        <input type="tel" maxlength="11" placeholder="手机号">
        <span class="btn">获取验证码</span>
    </div>
    <div class="bot">
        <input type="tel" maxlength="11" placeholder="验证码">
    </div>
    <span class="text">温馨提示：未注册硅谷外卖帐号的手机号，登录时将自动注册，且代表已同意<a href="javascript;:"> 《用户服务协议》</a></span>
    <button class="btn-submit">登录</button>
    <a href="javascript:;" class="guanyu">关于我们</a>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>
a{
    text-decoration: none;
    color: black;

}
input{
    display: inline-block;
    border:1px solid #7d7171bb;
    background-color: rgb(245, 241, 242);
    width: 280px;
    height: 40px;
    border-radius: 3px;
    padding-left: 10px;
    
}
input:focus{
    
    outline-color: #02a774;
}
.btn{
    margin-left: -90px;
    font-size: 14px;
    color: rgba(186, 192, 192, 0.692);
}
.bot input{
    margin-top: 20px;
}
.text{
    margin-top: 10px;
    display: inline-block;
    width: 280px;
    font-size: 12px;
    color: #999;
}
.text>a{
   color: #02a774;
}

/* 登录按钮 */
.btn-submit{
    display: block;
    width: 280px;
    height: 42px;
    margin-top: 30px;
    border-radius: 4px;
    background: #4cd96f;
    color: #fff;
    text-align: center;
    font-size: 16px;
    line-height: 42px;
    border: 0;
}
.guanyu{
    display: inline-block;
  margin-left: 115px;
    margin-top: 10px;
    font-size: 12px;
    color: rgba(186, 192, 192, 0.797);
}
</style>