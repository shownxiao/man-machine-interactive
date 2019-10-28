<template>
    <div class="partner-view">
        <div class="partner-title">
            <p style="font-size: 24px;">COOPERATIVE PARTNER</p>
            <p>战 略 合 作 伙 伴</p>
        </div>
        <div class="partner-card">
            <el-row>
                <el-col :span="4" v-for="(o, index) in 3" :key="o" :offset="index > 0 ? 4 : 0">
                    <el-card :body-style="{ padding: '0px' }" shadow="hover" class="partner">
                        <img :src='headerimgList[o - 1].url' class="image">
                        <div class="partner-name">
                            <b>{{headerimgList[o - 1].name}}</b>
                        </div>
                    </el-card>
                </el-col>
            </el-row>
        </div>
    </div>
</template>

<script>
/* eslint-disable */
import headerImg1 from '@/assets/人机图片/战略合作伙伴1.jpg'
import headerImg2 from '@/assets/人机图片/战略合作伙伴2.jpg'
import headerImg3 from '@/assets/人机图片/战略合作伙伴3.jpg'
export default {
    name: 'partner',
    data() {
        return {
            headerimgList: [
                {name: '中国农业科学院茶叶研究所', url: headerImg1},
                {name: '湖南省茶叶研究所', url: headerImg2},
                {name: '中南大学', url: headerImg3}
            ]
        }
    }
}
</script>
<style scoped>
    .partner-name {
        width: 100%;
        text-align: center;
        font-weight: 600;
        font-size: 20px;
        padding-top: 20px;
        padding-bottom: 20px;
    }

    .partner {
        width: 300px;
    }
    .partner-view {
        width: 100%;
        height: 650px;
        background-color: rgb(236, 238, 242);
    }

    .partner-title {
        width: 1000px;
        margin: 0 auto;
        text-align: center;
        height: 200px;
        padding-top: 50px;
    }

    .partner-card {
        width: 1080px;
        margin: 0 auto;
        padding-left: 70px;
    }
  
    .bottom {
        margin-top: 13px;
        line-height: 12px;
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