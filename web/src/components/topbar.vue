<script setup>
import Search from './search.vue';
import Avatar from './avatar.vue';
</script>

<template>
  <div class="topbar">
        <div class="topbar-left">
        <div class="logo"></div>
        <div class="site-name">校园论坛</div>
      </div>
      <div class="topbar-center">
          <span class="active">广场</span>
          <span>版块</span>
          <span>活动</span>
          <span>二手</span>
          <span>排行</span>
          <span>帮助</span>
      </div>

      <div class="topbar-right">
        <!-- 搜索栏 -->
        <Search></Search>
          <div class="icon-btn">信</div>
          <!-- 头像avatar -->
          <Avatar></Avatar>

      </div>
  </div>
</template>

<style scoped>
.topbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 60px;
  padding: 0 20px;
  background-color: #ffffff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}
.topbar-left {
  display: flex;
  align-items: center;
}
.logo {
  border-radius: 15%;
  border: 1px solid #5c5a5a;
  width: 40px;
  height: 40px;
  background-image: url('@/assets/logo.png');
  background-size: cover;
  margin-right: 10px;
}
.site-name {
  font-size: 20px;
  font-weight: bold;
}
.topbar-center {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
  font-size: 16px;
}
.topbar-center .active {
  font-weight: bold;
  color: #409eff;
}
.topbar-right {
  display: flex;
  align-items: center;
  gap: 10px;
}

.icon-btn {
  width: 32px;
  height: 32px;
  background-color: #dedfe1;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}

</style>
