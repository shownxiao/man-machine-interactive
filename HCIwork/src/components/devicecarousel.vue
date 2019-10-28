<template>
    <div class="device-container">
        <div class="content-view">
            <p style="margin: 0;">THINKING OF INDESTRIALIZATION CREATE INELLIGENT HIGH-END DEVICES INTELLIGENT HIGH-END INDUSTRIAL INOVATION</p>
            <p style="font-size: 20px;">用 工 业 思 维 打 造 智 能 化 高 端 设 备</p>
        </div>
        <div class="carousel-view">
            <el-carousel :interval="1000000" type="card" height="460px">
                <el-carousel-item v-for="item in 7" :key="item" class="card-item">
                    <el-card :body-style="{ padding: '0px' }" shadow="hover">
                        <img :src='headerimgList[item - 1].url' class="carousel-image"/>
                        <div style="padding: 14px;">
                            <p>{{headerimgList[item - 1].name}}</p>
                        </div>
                    </el-card>
                </el-carousel-item>
            </el-carousel>
        </div>
    </div>
</template>
<script>
/* eslint-disable */ 
import headerImg1 from '@/assets/image/扁茶生产线.jpg'
import headerImg2 from '@/assets/image/红茶生产线.jpg'
import headerImg3 from '@/assets/image/多功能绿茶.jpg'
import headerImg4 from '@/assets/image/香茶生产线.jpg'
import headerImg5 from '@/assets/image/炒绿茶生产线.jpg'
import headerImg6 from '@/assets/image/红绿茶兼制生产线.jpg'
import headerImg7 from '@/assets/image/颗粒型绿茶生产线.png'
export default {
    name: 'devicecarousel',
    data() {
        return {
            headerimgList: [
                {name: '扁茶生产线', url: headerImg1},
                {name: '红茶生产线', url: headerImg2},
                {name: '多动能绿茶', url: headerImg3},
                {name: '香茶生产线', url: headerImg4},
                {name: '炒绿茶生产线', url: headerImg5},
                {name: '红绿茶兼制生产线', url: headerImg6},
                {name: '颗粒型绿茶生产线', url: headerImg7},
            ]
        }
    }
}
</script>
<style>

  .carousel-view {
    height: 500px;
    width: 100%;
    text-align: center;
    width: 1000px;
    margin: 0 auto;
  }

  .card-item {
    margin: 0 auto;
    width: 50%;
  }

  .carousel-image {
      width: 100%;
      height: 100%;
  }

  .device-container {
      margin: 0 auto;
      text-align: center;
      width: 100%;
      background-color: rgb(236, 238, 241);
      padding-bottom: 50px;
  }

  .content-view {
      font-weight: 100;
      padding-top: 100px;
      padding-bottom: 50px;
  }

  .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 200px;
    margin: 0;
  }
  
  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }
  
  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }

  .time {
    font-size: 13px;
    color: #999;
  }
  
  .bottom {
    margin-top: 13px;
    line-height: 12px;
  }

  .button {
    padding: 0;
    float: right;
  }

  .image {
    width: 100%;
    display: block;
  }

  .clearfix:before,
  .clearfix:after {
      display: table;
      content: "";
  }
  
  .clearfix:after {
      clear: both
  }
</style>