<template>
  <div id="app">
  <router-view></router-view>
  <FooterGuide v-show="$route.meta.showFooter"></FooterGuide>
  </div>
  </template>
  <script>
  import FooterGuide from './components/FooterGuide/FooterGuide.vue'
  export default {
  components: {
  FooterGuide
  }
  }
  </script>
  <style scoped>
  *{
    padding: 0px;
    margin: 0px;
  }
  #app{
    margin: 0;
    padding: 0;
    width: 100%;
    height: 100%;
    /* margin-left: -16px; */
    
    height: 1200px;
    /* background-color: rgb(249, 245, 246); */
    /* background-color: pink; */


  }
  </style>