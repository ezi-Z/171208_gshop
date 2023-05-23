<template>
    <div>
    
     <div class="HeaderTop">
     <p class="title">{{ title }}</p>
    </div>
    <img src="../../common/images/order/person.png" alt="">
    <div class="text">登陆后查看外卖订单</div>
    <button @click="goTo">立即登录</button>
    </div>
  </template>
  
  <script>
  export default {
  
    data(){
      return {

        title:'订单列表'
      }
    },
    components:{
    },
    methods:{
      goTo(){
        console.log('123');
        this.$router.push('/login')
      }
    }
  }
  </script>
  

  <style scoped>

.HeaderTop{
  color: white;
  position: fixed;
        left: 0;
        top: 0;
        width :100%;
        height: 45px;
        background-color: #02a774;
}
.title{
/* position: absolute;
left: 50%;
transform: translateX(-50%); */

text-align: center;
}
img{
  margin-top:100px ;
  margin-left: 50px;
}
.text{
  margin-left: 120px;
  color: #d8d0d0;
}
button{
  color: white;
  width: 96px;
  height: 40px;
  background-color: #02a774;
  border: none;
  border-radius: 3px;
  margin-left: 140px;
  margin-top: 20px;
}
</style>