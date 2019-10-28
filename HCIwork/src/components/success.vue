<template>
    <div class="success-view">
        <div style="width: 100%; height: 200px;">
        </div>
        <div class="success-card-container">
            <div class="success-title">
                <p style="font-size: 32px; padding-top: 20px;">THERE CHOSE US</p>
                <b>他  们  选  择  我  们</b>
            </div>
            <div class="success-second-title">
                <p style="font-size: 24px;">SUCCESSFUL CASE</p>
                <p>成 功 案 例</p>
            </div>
            <div class="carousel-view">
                <el-carousel :interval="1000000" type="card" height="460px">
                    <el-carousel-item v-for="item in 5" :key="item" class="card-item">
                        <el-card :body-style="{ padding: '0px' }" shadow="hover">
                            <img :src='headerimgList[item - 1].url' class="carousel-image"/>
                            <div class="absolute-title">
                                <p>{{headerimgList[item - 1].name}}</p>
                            </div>
                            <div style="padding: 14px;">
                                <p>{{headerimgList[item - 1].content}}</p>
                            </div>
                        </el-card>
                    </el-carousel-item>
                </el-carousel>
            </div>
        </div>
    </div>
</template>

<script>
/* eslint-disable */ 
import headerImg1 from '@/assets/image/湖南华莱生物科技.jpg'
import headerImg2 from '@/assets/image/临沂山松生物.jpg'
import headerImg3 from '@/assets/image/中国茶叶研究所.jpg'
import headerImg4 from '@/assets/image/印江土家族苗族自治县勇创茶叶.jpg'
import headerImg5 from '@/assets/image/川红重庆茶叶集团.jpg'
export default {
    name: 'success',
    data() {
        return {
            headerimgList: [
                {name: '湖南华莱生物科技', url: headerImg1, content: '湖南华莱生物全自动多功能红绿黑茶生产效果图'},
                {name: '临沂山松生物', url: headerImg2, content: '临沂山松生物'},
                {name: '中国茶叶研究所', url: headerImg3, content: '茶鲜叶处理实验平台-炒干实验平台-烘干实验平台-条形茶做形平台'},
                {name: '印江土家族苗族自治县勇创茶叶', url: headerImg4, content: '印江土家族苗族自治县勇创茶叶'},
                {name: '川红重庆茶叶集团', url: headerImg5, content: '川红重庆茶叶集团'}
            ]
        }
    }
}
</script>

<style scoped>
  .success-second-title {
      padding-top: 20px;
      padding-bottom: 20px;
      text-align: center;
  }

  .absolute-title {
      position: absolute;
      top: 293px;
      width: 100%;
      height: 80px;
      left: 0;
      z-index: 10;
      background-color: rgb(109, 159, 169);
      opacity: 0.8;
      color: white;
      font-size: 20px;
  }

   .carousel-image {
      position: relative; 
   }
  .success-view {
      background-color: white;
      background: url('../assets/image/道路的那张图片.jpg') top left no-repeat;
      background-size: 100%;
      width: 100%;
      height: 1050px;
  }

  .success-card-container {
      background-color: white;
      height: 500px;
      width: 1000px;
      margin: 0 auto;
      border-radius: 10px;
  }

  .success-title {
      height: 150px;
      text-align: center;
      background-color: rgb(109, 159, 169);
      color: white;
  }

</style>