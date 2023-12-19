<template>
  <div id="app">
      <!-- header 头部区域-->
      <div style="height: 60px; line-height: 60px; background-color: white; margin-bottom: 2px">
          <img src="@/assets/logo.png" alt="" style="width: 40px; position: relative; top: 10px;left: 20px">
          <span style="margin-left: 30px;font-size: 24px">图书管理系统</span>
      </div>

      <!-- 侧边栏和主体 -->
      <div style="display: flex">
          <!-- 侧边栏导航 -->
          <div style="width: 200px; min-height: calc(100vh - 62px); overflow: hidden; margin-right: 2px; background-color: white">
              <el-menu :default-active="$route.path" :default-openeds="['1']" router class="el-menu-demo">
                  <el-menu-item index="/">
                      <i class="el-icon-eleme"></i>
                      <span>首页</span>
                  </el-menu-item>
                  <el-submenu index="1">
                      <template slot="title">
                          <i class="el-icon-info"></i>
                          <span>关于页面</span>
                      </template>
                      <el-menu-item index="/about">
                          <i class="el-icon-question"></i>
                          <span>关于详情</span>
                      </el-menu-item>
                  </el-submenu>
              </el-menu>

          </div>





          <!-- 主体内容 -->
          <div style="flex: 1; background-color: white">
              <router-view/>
          </div>
      </div>

  </div>
</template>

<script setup>
</script>
