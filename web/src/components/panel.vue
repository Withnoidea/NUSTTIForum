<template>
  <div class="panel">
      <el-card style="max-width: 480px">
      <template #header>
        <div class="card-header">
          <span>校园公告</span>
        </div>
      </template>
      <p>【教务处】本周选课时间调整说明</p>
      <p>【学工处】关于寒假安全事项提醒</p>
      <p>【图书馆】考试周延长开放时间通知</p>
    </el-card>
      <el-card style="max-width: 480px">
      <template #header>
        <div class="card-header">
          <span>今日热点帖子</span>
        </div>
      </template>
      <p>1. 期末复习资料大合集（附下载链接示意）</p>
      <p>2. 校园二手书集市活动预告</p>
      <p>3. 宿舍电费省钱经验分享</p>
      <p>4. 社团招新：编程社 / 演讲社</p>
      <p>5. 树洞：关于毕业的那些话</p>
    </el-card>
      <el-card style="max-width: 480px">
      <template #header>
        <div class="card-header">
          <span>热门话题标签</span>
        </div>
      </template>
      <div class="tag-cloud">
        <el-tag type="primary" size="medium">#期末考试</el-tag>
        <el-tag type="success" size="medium">#资料分享</el-tag>
        <el-tag type="info" size="medium">#校园美食</el-tag>
        <el-tag type="warning" size="medium">#二手交易</el-tag>
        <el-tag type="danger" size="medium">#失物招领</el-tag>
        <el-tag type="primary" size="medium">#考研经验</el-tag>
        <el-tag type="success" size="medium">#社团活动</el-tag>
        <el-tag type="info" size="medium">#树洞</el-tag>
      </div>
    </el-card>
  </div>
</template>

<script>
</script>

<style scoped>

</style>