<template>
    <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
        <el-menu-item index="1">
            <img src="../assets/人机图片/logo.jpg" style="width: 170px; height:60px;">
        </el-menu-item>
        <el-menu-item index="2">首页</el-menu-item>
        <el-submenu index="3">
            <template slot="title">关于我们</template>
            <el-menu-item index="3-1">公司简介</el-menu-item>
            <el-menu-item index="3-2">配套事业部</el-menu-item>
            <el-menu-item index="3-3">长沙红点科技</el-menu-item>
            <el-menu-item index="3-4">企业文化</el-menu-item>
            <el-menu-item index="3-5">企业荣誉</el-menu-item>
            <el-menu-item index="3-6">员工风采</el-menu-item>
        </el-submenu>
        <el-submenu index="4">
            <template slot="title">产品中心</template>
            <el-menu-item index="4-1">非标产品</el-menu-item>
            <el-menu-item index="4-2">数据采集系统</el-menu-item>
            <el-menu-item index="4-3">单机模块</el-menu-item>
            <el-menu-item index="4-4">生产线</el-menu-item>
        </el-submenu>
        <el-submenu index="5">
            <template slot="title">新闻中心</template>
            <el-menu-item index="5-1">公司新闻</el-menu-item>
            <el-menu-item index="5-2">行业动态</el-menu-item>
            <el-menu-item index="5-3">媒体通告</el-menu-item>
            <el-menu-item index="5-4">通知公告</el-menu-item>
        </el-submenu>
        <el-submenu index="6">
            <template slot="title">营销与服务</template>
            <el-menu-item index="6-1">合作伙伴</el-menu-item>
            <el-menu-item index="6-2">客户案例</el-menu-item>
            <el-menu-item index="6-3">服务理念</el-menu-item>
            <el-menu-item index="6-4">营销网络</el-menu-item>
            <el-menu-item index="6-5">资料下载</el-menu-item>
        </el-submenu>
        <el-submenu index="7">
            <template slot="title">招贤纳士</template>
            <el-menu-item index="7-1">人才政策</el-menu-item>
            <el-menu-item index="7-2">人才招聘</el-menu-item>
        </el-submenu>
        <el-menu-item index="8">联系我们</el-menu-item>
        <el-menu-item index="9">English</el-menu-item>
    </el-menu>
</template>
<script>
/* eslint-disable */ 
  export default {
    name: 'myheader',
    data() {
      return {
        activeIndex: '2',
      }
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>
<style scoped>
    .header-title {
        text-align: center;
    }
</style>