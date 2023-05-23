<template>
    <div>

     <div class="HeaderTop">
     <p class="title">{{ title }}</p>
      <div class="search">
        <input type="text" placeholder="请输入商品或商家名称" class="search-s">
        <button class="submit" @click="subclick">提交</button>
      </div>
   

    </div>
    </div>
  </template>
  
  <script>
  export default {
  
    data(){
      return {

        title:'搜索'
      }
    },
    components:{
   
    },
    methods :{
      subclick(){
        
        this.$router.push('/msite')
        console.log('点击触发了函数');
      }
    }
  }
  </script>
  

  <style scoped>
  *{
    margin: 0;
    padding: 0;
  }
.HeaderTop{
  position: fixed;
        left: 0;
        top: 0;
        width :100%;
        height: 45px;
        background-color: #02a774;
        color: white;
        
}
.title{
line-height: 45px;
text-align: center;
}
.search{

  width: 100%;
  height: 59px;
  background-color: white;
}
.submit{
  display: inline-block;
  color: black;
  width: 68px;
  height: 32px;
  background-color: #02a774;
  color: white;
  text-align: center;
  line-height: 27px;
  border: 4px solid #02a774;
}
.search-s{
  width: 296px;
  height: 35px;
  border: none;
  background: #f2f2f2;
margin: 10px 5px 5px 10px;
}
</style>