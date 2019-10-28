<template>
    <div class="customer-view">
        <div class="customer-title">
            <p style="font-size: 24px;">CUSTOMER UNIT</p>
            <p>客 户 单 位</p>
        </div>
        <div class="customer-card">
            <el-row>
                <el-col :span="2" v-for="(o, index) in 5" :key="o" :offset="index > 0 ? 3 : 0">
                    <el-card :body-style="{ padding: '0px' }" shadow="hover" class="customer">
                        <img :src='headerimgList[o - 1]' class="image">
                    </el-card>
                </el-col>
            </el-row>
        </div>
    </div>
</template>
<script>
/* eslint-disable */ 
import headerImg1 from '@/assets/人机图片/客户单位.jpg'
import headerImg2 from '@/assets/人机图片/客户单位2.jpg'
import headerImg3 from '@/assets/人机图片/客户单位3.jpg'
import headerImg4 from '@/assets/人机图片/客户单位4.jpg'
import headerImg5 from '@/assets/人机图片/客户单位5.jpg'
export default {
    name: 'customer',
    data() {
        return {
            headerimgList: [
                headerImg1, headerImg2, headerImg3, headerImg4, headerImg5
            ]
        }
    }
}
</script>
<style scoped>
    .customer {
        width: 180px;
    }
    .customer-card {
        width: 1000px;
        margin: 0 auto;
    }
    .customer-view {
        width: 100%;
        background-color: white;
        background: url('../assets/人机图片/ban3.jpg') top left no-repeat;
        background-size: 100% 100%;
        padding-bottom: 80px;
    }

    .customer-title {
        width: 1000px;
        margin: 0 auto;
        text-align: center;
        height: 180px;
        padding-top: 10px;
        color: white;
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