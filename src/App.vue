<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
import './font/style.css'
export default {
  name: 'App',
  components: {

  }
}
</script>

<style>
  /* CSS reset */
  html{color:#000;background:#fff;-webkit-tap-highlight-color:rgba(0,0,0,0);font-family: 'PingFangSC-Thin',"Microsoft YaHei","微软雅黑","sans-serif";font-size: 12px;}
  body,div,dl,dt,dd,ul,ol,li,h1,h2,h3,h4,form,input,button,textarea,p,th,td,strong{padding:0;margin:0;font-family: 'PingFangSC-Thin',"Microsoft YaHei","微软雅黑","sans-serif";}
  table{border-collapse:collapse;border-spacing:0;}
  img{border:0;}
  a{text-decoration:none; color:#999; outline:none;}/*此处待添加默认链接颜色*/
  var,em,strong{font-style:normal;}
  em,strong,th,var{font-style:inherit;font-weight:inherit;}
  li{list-style:none;}
  caption,th{text-align:left;}
  h1,h2,h3,h4{font-size:100%;font-weight:normal;}
  input,button,textarea,select,option{font-family:inherit; font-size:inherit;font-style:inherit;font-weight:inherit;}
  input,button,textarea,select{*font-size:100%;}
  .clearfix:after {content:"\200B"; display:block; height:0; clear:both; }
  .clearfix { *zoom:1; }

  html {
    position: relative;
    width: 100%;
    overflow: hidden;
    overflow-y: scroll;
  }
  #app {
  }
  .pc {
    width: 100%;
    overflow: hidden;
  }
  .selection {
    position: relative;
    width: 100%;
    height: 100vh;
    overflow: hidden;
  }
  /*侧边返回顶部*/
  .sider-nav {
    position: fixed;
    right: 2.45vw;
    top: 50vh;
    z-index: 1000;
  }
  .sider-nav ul {
    cursor: pointer;
  }
  .sider-nav ul li:hover {
    background-color: #fff;
    color: #161519;
    -webkit-transition: all .2s;
    transition: all .2s;
  }
  .sider-nav ul:hover li p {
    width: 9.7vw;
    padding-left: 0.6vw;
    -webkit-transition: all .3s;
    transition: all .3s;
  }
  .sider-nav li {
    height: 2.5vw;
    padding: 0 0.6vw;
    color: #fff;
    line-height: 2.5vw;
    font-size: 0.63vw;
    background: #161519;
  }
  .sider-nav p {
    float: left;
    overflow: hidden;
    width: 0vw;
    height: 2.5vw;
    font-size: 0.63vw;
    font-family: 'PingFangSC-Light';
  }
  .sider-nav .nav-time {
    line-height: 1.5vw;
  }
  .sider-nav .nav-time span {
    display: block;
    margin-top: -0.4vw;
    font-size: 0.52vw;
  }
  .sider-nav i {
    float: left;
    text-align: center;
    line-height: 2.5vw;
    font-size: 1.56vw;
  }
  .sider-nav .oneline {
    position: relative;
  }
  .sider-nav .oneline:after {
    position: absolute;
    top: 0;
    content: '';
    width: 1.04vw;
    height: 1.77vw;
    background: url('../src/assets/8.svg') center center no-repeat;
    background-size: 100% 100%;
  }

  .down-con {
    position: absolute;
    left: 0;
    width: 100%;
    bottom: 8.7vh;
  }
  .down {
    position: relative;
    margin: 0 auto 1.59vh;
    width: 2.29vw;
    height: 3.75vw;
    background: url('../src/assets/4.svg') center center no-repeat;
    background-size: 100% 100%;
  }
  .down:after {
    position: absolute;
    left: 0;
    right: 0;
    bottom: 0;
    top: 1.6vh;
    margin: 0 auto;
    content: '';
    width: 0.26vw;
    height: 0.78vw;
    background: url('../src/assets/5.svg') center center no-repeat;
    background-size: 100% 100%;
    cursor: pointer;
    -webkit-animation: fall 1.2s infinite;
    animation: fall 1.2s infinite;
  }
  .slidedown {
    margin: 0 auto;
    width: 11.41vw;
    height: 2.76vw;
    line-height: 2.76vw;
    font-size: 1.04vw;
    cursor: pointer;
  }

  .title {
    position: relative;
    color: #000;
    text-align: left;
    font-size: 1.82vw;
    font-family: 'PingFangSC-Semibold';
  }
  
  .title:after {
    content: "";
    position: absolute;
    bottom: -2.5vh;
    left: 0.2vw;
    width: 1.88vw;
    height: 0.16vw;
    background: #5BB8DE;
  }

  .more {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 6.41vw;
    height: 2.34vw;
    background: url('../src/assets/11.svg') center center no-repeat;
    background-size: 100% 100%;

  }
  .more i {
    color: #5BB8DE;
    font-size: 1.15vw;
    -webkit-transition: all .8s;
      transition: all .8s;
  }
  .more span {
    margin-right: 0.42vw;
    color: #FFF;
    font-size: 0.73vw;
    font-family: 'PingFangSC-Regular';
  }
  .more:hover i {
    color: #fff;
    -webkit-transition: all .8s;
      transition: all .8s;
  }


  .mob {
    display: none;
  }

  /*向下效果*/
  @-webkit-keyframes fall {
    0% {
      -webkit-transform: translateY(-10px);
      -moz-transform: translateY(-10px);
      -ms-transform: translateY(-10px);
      -o-transform: translateY(-10px);
    }
    60% {
      -webkit-transform: translateY(15px);
      -moz-transform: translateY(15px);
      -ms-transform: translateY(15px);
      -o-transform: translateY(15px);
    }
    100% {
      -webkit-transform: translateY(-10px);
      -moz-transform: translateY(-10px);
      -ms-transform: translateY(-10px);
      -o-transform: translateY(-10px);
    }
  }
  @keyframes fall {
    0% {
      -webkit-transform: translateY(-10px);
      -moz-transform: translateY(-10px);
      -ms-transform: translateY(-10px);
      -o-transform: translateY(-10px);
    }
    60% {
      -webkit-transform: translateY(15px);
      -moz-transform: translateY(15px);
      -ms-transform: translateY(15px);
      -o-transform: translateY(15px);
    }
    100% {
      -webkit-transform: translateY(-10px);
      -moz-transform: translateY(-10px);
      -ms-transform: translateY(-10px);
      -o-transform: translateY(-10px);
    }
  }

  /*漂浮*/
  @-webkit-keyframes float_01 {
    0% {
      -webkit-transform: translateY(5px);
      -moz-transform: translateY(5px);
      -ms-transform: translateY(5px);
      -o-transform: translateY(5px);
    }
    50% {
      -webkit-transform: translateY(-5px);
      -moz-transform: translateY(-5px);
      -ms-transform: translateY(-5px);
      -o-transform: translateY(-5px);
    }
    100% {
      -webkit-transform: translateY(5px);
      -moz-transform: translateY(5px);
      -ms-transform: translateY(5px);
      -o-transform: translateY(5px);
    }
  }
  @keyframes float_01 {
    0% {
      -webkit-transform: translateY(5px);
      -moz-transform: translateY(5px);
      -ms-transform: translateY(5px);
      -o-transform: translateY(5px);
    }
    50% {
      -webkit-transform: translateY(-5px);
      -moz-transform: translateY(-5px);
      -ms-transform: translateY(-5px);
      -o-transform: translateY(-5px);
    }
    100% {
      -webkit-transform: translateY(5px);
      -moz-transform: translateY(5px);
      -ms-transform: translateY(5px);
      -o-transform: translateY(5px);
    }
  }
  @-webkit-keyframes float_02 {
    0% {
      -webkit-transform: translateY(10px);
      -moz-transform: translateY(10px);
      -ms-transform: translateY(10px);
      -o-transform: translateY(10px);
    }
    50% {
      -webkit-transform: translateY(-10px);
      -moz-transform: translateY(-10px);
      -ms-transform: translateY(-10px);
      -o-transform: translateY(-10px);
    }
    100% {
      -webkit-transform: translateY(10px);
      -moz-transform: translateY(10px);
      -ms-transform: translateY(10px);
      -o-transform: translateY(10px);
    }
  }
  @keyframes float_02 {
    0% {
      -webkit-transform: translateY(10px);
      -moz-transform: translateY(10px);
      -ms-transform: translateY(10px);
      -o-transform: translateY(10px);
    }
    50% {
      -webkit-transform: translateY(-10px);
      -moz-transform: translateY(-10px);
      -ms-transform: translateY(-10px);
      -o-transform: translateY(-10px);
    }
    100% {
      -webkit-transform: translateY(10px);
      -moz-transform: translateY(10px);
      -ms-transform: translateY(10px);
      -o-transform: translateY(10px);
    }
  }
  @-webkit-keyframes float_03 {
     0% {
      -webkit-transform: translateY(30px);
      -moz-transform: translateY(30px);
      -ms-transform: translateY(30px);
      -o-transform: translateY(30px);
    }
    50% {
      -webkit-transform: translateY(-30px);
      -moz-transform: translateY(-30px);
      -ms-transform: translateY(-30px);
      -o-transform: translateY(-30px);
    }
    100% {
      -webkit-transform: translateY(30px);
      -moz-transform: translateY(30px);
      -ms-transform: translateY(30px);
      -o-transform: translateY(30px);
    }
  }
  @keyframes float_03 {
    0% {
      -webkit-transform: translateY(30px);
      -moz-transform: translateY(30px);
      -ms-transform: translateY(30px);
      -o-transform: translateY(30px);
    }
    50% {
      -webkit-transform: translateY(-30px);
      -moz-transform: translateY(-30px);
      -ms-transform: translateY(-30px);
      -o-transform: translateY(-30px);
    }
    100% {
      -webkit-transform: translateY(30px);
      -moz-transform: translateY(30px);
      -ms-transform: translateY(30px);
      -o-transform: translateY(30px);
    }
  }
  @-webkit-keyframes float_04 {
    0% {
      -webkit-transform: translateY(15px);
      -moz-transform: translateY(15px);
      -ms-transform: translateY(15px);
      -o-transform: translateY(15px);
    }
    50% {
      -webkit-transform: translateY(-15px);
      -moz-transform: translateY(-15px);
      -ms-transform: translateY(-15px);
      -o-transform: translateY(-15px);
    }
    100% {
      -webkit-transform: translateY(15px);
      -moz-transform: translateY(15px);
      -ms-transform: translateY(15px);
      -o-transform: translateY(15px);
    }
  }
  @keyframes float_04 {
    0% {
      -webkit-transform: translateY(15px);
      -moz-transform: translateY(15px);
      -ms-transform: translateY(15px);
      -o-transform: translateY(15px);
    }
    50% {
      -webkit-transform: translateY(-15px);
      -moz-transform: translateY(-15px);
      -ms-transform: translateY(-15px);
      -o-transform: translateY(-15px);
    }
    100% {
      -webkit-transform: translateY(15px);
      -moz-transform: translateY(15px);
      -ms-transform: translateY(15px);
      -o-transform: translateY(15px);
    }
  }

  @media screen and (max-width: 750px) {
    .mob {
      display: block;
    }
    .pc {
      display: none;
    }
    .down {
      margin: 0 auto 2.51vh;
      width: 9.6vw;
      height: 15.73vw;
    }
    .down:after {
      top: 2.6vh;
      width: 1.07vw;
      height: 3.2vw;
    }
    .slidedown {
      width: 100%;
      height: 4.76vw;
      line-height: 4.76vw;      
      font-size: 4.27vw;
    }
    .title {
      line-height: 9.34vw;
      font-size: 8vw;
    }
    
    .title:after {
      bottom: -5.91vh;
      margin: 0 auto;
      width: 14.93vw;
      height: 0.53vw;
    }
    .discr {
      margin-top: 11.52vh;
      font-size: 5.33vw;
    }

    .more {
      width: 28.53vw;
      height: 10.4vw;
    }
    .more i {
      font-size: 5vw;
    }
    .more span {
      margin-right: 2.13vw;
      font-size: 3.73vw;
    }
    .title:after {
      left: 1vw;
    }

    /*返回顶部*/
    .tops {
      display: none;
      position: fixed;
      right: 2.93vw;
      bottom: 26.27vh;
      width: 11.47vw;
      height: 11.47vw;
      background: url('../src/assets/22.svg') center center no-repeat;
      background-size: 100% 100%;
      z-index: 99999999;
    }
  }
</style>
