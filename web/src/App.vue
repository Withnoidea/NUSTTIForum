<script setup>
import Topbar from './components/topbar.vue'
import Navi from './components/navi.vue'
import Posteditor from './components/posteditor.vue';
import Panel from './components/panel.vue';
</script>

<template>
    <Topbar />
    <div class="body">
        <el-row :gutter="20">
            <el-col :span="4">
                <Navi/>
            </el-col>
            <el-col :span="14">
                <Posteditor/>
            </el-col>
            <el-col :span="6">
                <Panel/>
            </el-col>
        </el-row>
    </div>
    <div class="footer">
        校园论坛 &copy; 2025 NUSTTI All Rights Reserved.
    </div>
</template>

<style scoped>
.body {
    gap: 20px;
    padding: 20px;
}
.el-row {
  margin-bottom: 20px;
}
.el-row:last-child {
  margin-bottom: 0;
}
.el-col {
  border-radius: 4px;
}
.footer {
    text-align: center;
    padding: 15px 0;
    background-color: #f5f5f5;
    color: #878585;
    font-size: 14px;
    margin-top: 20px;
}
</style>
