<template>
  <div id="app">
    <div class="header-container">
      <div class="header-box">
        <myheader></myheader>
      </div>
    </div>
    <div class="top-button">
        <el-button type="primary" icon="el-icon-upload2" circle id="toTop"></el-button>
    </div>
    <div class="header-carousel-container">
      <headercarousel></headercarousel>
    </div>
    <div class="device-carousel-container">
      <devicecarousel></devicecarousel>
    </div>
    <div class="success-container">
      <success></success>
    </div>
    <div class="partner-container">
      <partner></partner>
    </div>
    <div class="customer-contianer">
      <customer></customer>
    </div>
    <div class="message-container">
      <message></message>
    </div>
    <div class="footer-container">
      <footerimg></footerimg>
    </div>
  </div>
</template>

<script>
/* eslint-disable */
import myheader from './components/header'
import headercarousel from './components/headercarousel'
import devicecarousel from './components/devicecarousel'
import success from './components/success'
import partner from './components/partner'
import customer from './components/customer'
import footerimg from './components/footer'
import message from './components/message'

window.onload = function(){
  var btn = document.getElementById("toTop");
  var timer = null;
  var oScroll = true;
  window.onscroll = function(){
    if(!oScroll){
      clearInterval(timer);
    }
    oScroll = false;
  }
  btn.onclick = function(){
    timer = setInterval(function(){
      var oTop = document.documentElement.scrollTop || document.body.scrollTop;
      var ispeed = Math.floor(-oTop / 7);
      document.documentElement.scrollTop = document.body.scrollTop = oTop + ispeed;
      oScroll = true;
      if(oTop == 0){
        clearInterval(timer);
      }
    },30);
  }
}
export default {
  name: 'App',
  components: {
    myheader: myheader,
    headercarousel: headercarousel,
    devicecarousel: devicecarousel,
    success: success,
    partner: partner,
    customer: customer,
    message: message,
    footerimg: footerimg
  }
}
</script>

<style scoped>
  .header-carousel-container {
    height: 500px;
  }

  .top-button {
    position:fixed;
    right: 20px;
    bottom: 40px;
  }

  .header-container {
    position: sticky;
    position: -webkit-sticky;
    top: 0;
    z-index: 100;
    width: 100%;
    /* position: absolute; */
    opacity: 0.8;
    border-bottom: 2px solid grey;
    background-color: #fff;
    -moz-box-shadow:0px 2px 13px #333333; -webkit-box-shadow:0px 2px 13px #333333; box-shadow:0px 2px 13px #333333;
  }

  .header-box {
    text-align: center;
    margin: 0 auto;
    width: 1100px;
  }

  .footer-container {
    margin: 0;
  }

</style>