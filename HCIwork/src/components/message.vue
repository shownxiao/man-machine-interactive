<template>
    <div class="message-view">
        <div class="message-title">
            <p style="font-size: 24px;">THE LATEST KNOWN DYNAMIC COMPANY</p>
            <p>公 司 最 新 动 态 周 知</p>
        </div>
        <div class="message-box">
            <div class="message-left">
                <div class="message-import" style="height: 160px; margin-bottom: 20px;">
                    <div class="date" style="padding-top: 30px;">
                        <p style="font-size: 54px; margin: 0">22</p>
                        <p style="font-size: 12px;">2018.10</p>
                    </div>
                    <img src="@/assets/人机图片/国家茶叶加工装备研发专业中心.jpg"/>
                </div>
                <b style="font-size: 18px; color: rgb(109, 159, 169)">我公司被评为“国家茶叶加工装备研发专业中心”</b>
                <p style="margin-top: 20px; font-size: 14px;">2018年8月我司获评“国家农产品加工技术研发专业中心”。</p>
            </div>
            <div class="message-right">
                <div class="message-import">
                    <div class="date">
                        <p style="font-size: 48px; margin: 0">19</p>
                        <p style="font-size: 12px; margin: 0 auto;">2018.01</p>
                    </div>
                    <div class="content">
                        <p style="margin: 0">湘丰装备获得2017年湖南省战略性新兴产业科技攻..</p>
                        <p style="margin-top: 16px; font-size: 12px;">近日，湖南省科技厅与湖南省经信委联合下文公布2017年湖南省战略性新兴产业科技攻关与重大科技成果转化项目项目名..</p>
                    </div>
                </div>
                <div class="message-import">
                    <div class="date">
                        <p style="font-size: 48px; margin: 0">19</p>
                        <p style="font-size: 12px; margin: 0 auto;">2018.01</p>
                    </div>
                    <div class="content">
                        <p style="margin: 0">台湾客户来湘丰装备考察</p>
                        <p style="margin-top: 16px; font-size: 12px;">2017年12月10日，我国台湾企业家林博士及丈夫罗博士在长沙市台办及长沙县台办相关同志的陪同下来到我公司考察。林..</p>
                    </div>
                </div>
                <div class="message-import">
                    <div class="date">
                        <p style="font-size: 48px; margin: 0">19</p>
                        <p style="font-size: 12px; margin: 0 auto;">2018.01</p>
                    </div>
                    <div class="content">
                        <p style="margin: 0">省经信委装备处来湘丰装备调研考察</p>
                        <p style="margin-top: 16px; font-size: 12px;">2018年1月12日，湖南省经济与信息化委员会装备处处长马天毅、副处长彭斌、肖辉、刘斌等一行来我公司考察，在公司首席..</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="button-view">
            <el-button type="primary" style="background-color: rgb(109, 159, 169);">更多信息</el-button>
        </div>
    </div>
</template>
<script>
/* eslint-disable */
export default {
    name: 'message',
    data() {
        return {

        }
    }
}
</script>
<style scoped>
    .button-view {
        margin: 0 auto;
        text-align: center;
    }

    .content {
        margin-left: 20px;
    }

    .date {
        text-align: center;
        width: 150px;
        height: 80px;
        color: rgb(109, 159, 169);
    }
    .message-import {
        display: flex;
        height: 100px;
    }

    .message-import img {
        width: 200px;
        height: 150px;
    }

    .message-left {
        width: 50%;
    }

    .message-right {
        width: 50%;
    }

    .message-box {
        width: 1000px;
        height: 300px;
        margin: 0 auto;
        display: flex;
    }

    .message-view {
        width: 100%;
        height: 650px;
        background-color: rgb(236, 238, 242);
    }

    .message-title {
        width: 1000px;
        margin: 0 auto;
        text-align: center;
        height: 200px;
        padding-top: 50px;
    }
</style>