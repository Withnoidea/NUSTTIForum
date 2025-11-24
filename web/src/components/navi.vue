<template>
  <el-row class="tac">
    <el-col :span="24">
      <h5 class="mb-2">版块导航</h5>
      <el-menu
        default-active="1"
        class="el-menu-vertical-demo"
        @open="handleOpen"
        @close="handleClose"
      >
        <el-menu-item index="1">
          <el-icon><icon-menu /></el-icon>
          <span>学习交流</span>
        </el-menu-item>
        <el-menu-item index="2">
          <el-icon><icon-menu /></el-icon>
          <span>课程讨论</span>
        </el-menu-item>
        <el-menu-item index="3">
          <el-icon><icon-menu /></el-icon>
          <span>考研 / 考公</span>
        </el-menu-item>
        <el-menu-item index="4">
          <el-icon><icon-menu /></el-icon>
          <span>校园生活</span>
        </el-menu-item>
        <el-menu-item index="5">
          <el-icon><icon-menu /></el-icon>
          <span>宿舍 / 食堂</span>
        </el-menu-item>
        <el-menu-item index="6">
          <el-icon><icon-menu /></el-icon>
          <span>社团活动</span>
        </el-menu-item>
        <el-menu-item index="7">
          <el-icon><icon-menu /></el-icon>
          <span>二手交易</span>
        </el-menu-item>
        <el-menu-item index="8">
          <el-icon><icon-menu /></el-icon>
          <span>失物招领</span>
        </el-menu-item>
        <el-menu-item index="9">
          <el-icon><icon-menu /></el-icon>
          <span>树洞专区</span>
        </el-menu-item>
      </el-menu>
    </el-col>
  </el-row>
</template>

<script lang="ts" setup>
import {
  Document,
  Menu as IconMenu,
  Location,
  Setting,
} from '@element-plus/icons-vue'

const handleOpen = (key: string, keyPath: string[]) => {
  console.log(key, keyPath)
}
const handleClose = (key: string, keyPath: string[]) => {
  console.log(key, keyPath)
}
</script>