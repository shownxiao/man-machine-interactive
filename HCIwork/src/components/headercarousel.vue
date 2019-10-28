<template>
  <el-carousel :interval="3000000" arrow="always" autoplay=false height="500px">
    <el-carousel-item v-for="item in 3" :key="item" class="header__container">
      <img :src='headerimgList[item - 1]' class="carousel-image"/>
    </el-carousel-item>
  </el-carousel>
</template>

<script>
/* eslint-disable */
import headerImg1 from '@/assets/image/追求卓越品质打造.jpg'
import headerImg2 from '@/assets/image/诚信立足.jpg'
import headerImg3 from '@/assets/image/湘丰智能装备茶叶生产线.jpg'

export default {
    name: 'headercarousel',
    data() {
        return {
            headerimgList: [
                headerImg1, headerImg2, headerImg3
            ]
        }
    }
}
</script>

<style>
  .el-carousel--horizontal {
    overflow-x: hidden;
  }

  .header__container {
      height: 500px;
      width: 100%;
  }
  .el-carousel__item {
      width: 100%;
  }

  .el-carousel__item image {
    color: #475669;
    font-size: 18px;
    opacity: 0.75;
    width: 100%;
    height: 50px;
  }
  
  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }
  
  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }

  .carousel-image {
      width: 100%;
      height: 100%;
  }
</style>