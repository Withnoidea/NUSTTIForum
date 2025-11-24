<template>
<div class="poster-editor">
    <el-input
      v-model="textarea2"
      style="width: 80%; height: 50px; "
      :autosize="{ minRows: 2, maxRows: 4 }"
      type="textarea"
      placeholder="有什么想和大家分享的？（标题和详细内容可在弹出的发帖页中填写"
    />
    <div style="display:flex; justify-content: space-between; align-items:center;">
      <div style="font-size:12px; color:#666;">选择版块 / 标签（示意）</div>
      <button class="btn-primary">发表帖子</button>
    </div>

    <!-- 筛选和排序 -->
    <div class="post-filter">
      <div class="filter">
        <span class="active">最新</span>
        <span>最热</span>
        <span>回复最多</span>
      </div>
      <div>共 1234 条帖子（示意）</div>
    </div>

    <!-- 卡片 -->
     <!-- 帖子卡片（示例1） -->
    <div class="post-card">
      <div class="post-title">[学习交流] 期末复习资料分享 & 复习群整理</div>
      <div class="post-meta">
        作者：某某同学 · 计算机学院 · 3小时前 · 浏览 256
      </div>
      <div class="post-tags">
        <span class="tag">#期末考试</span>
        <span class="tag">#资料分享</span>
      </div>
      <div class="post-meta" style="margin-bottom:6px;">
        这里是帖子内容摘要区域，只展示前面一小段内容，点击卡片进入详情页查看完整内容……
      </div>
      <div class="post-ops">
        <span>👍 32</span>
        <span>💬 18</span>
        <span>⭐ 收藏</span>
        <span style="margin-left:auto;">举报</span>
      </div>
    </div>

        <!-- 帖子卡片（示例2） -->
    <div class="post-card">
      <div class="post-title">[校园生活] 宿舍楼下新开的奶茶店怎么样？</div>
      <div class="post-meta">
        作者：匿名 · 经济学院 · 昨天 · 浏览 512
      </div>
      <div class="post-tags">
        <span class="tag">#校园美食</span>
        <span class="tag">#吐槽</span>
      </div>
      <div class="post-meta" style="margin-bottom:6px;">
        帖子摘要区域……点击进入详情页可查看图片和完整讨论。
      </div>
      <div class="post-ops">
        <span>👍 20</span>
        <span>💬 45</span>
        <span>⭐ 收藏</span>
        <span style="margin-left:auto;">举报</span>
      </div>
    </div>
</div>
  <!-- 分页 -->
    <el-pagination class="page-count" background layout="prev, pager, next" :total="1000" />
</template>

<script lang="ts" setup>
import { ref } from 'vue'

const textarea1 = ref('')
const textarea2 = ref('')
</script>

<style scoped>
.poster-editor {
  padding: 10px;
  border: 1px solid #e0e0e0;
  border-radius: 5px;
  background-color: #ffffff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}
.post-filter {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 15px;
  font-size: 14px;
  color: #555;
}
.filter span {
  margin-right: 15px;
  cursor: pointer;
}
.filter .active {
  font-weight: bold;
  color: #409eff;
}
.post-card {
  border: 1px solid #e0e0e0;
  border-radius: 5px;
  padding: 15px;
  margin-top: 15px;
  background-color: #fafafa;
}
.post-title {
  font-size: 16px;
  font-weight: bold;
  margin-bottom: 8px;
}
.post-meta {
  font-size: 12px;
  color: #888;
  margin-bottom: 6px;
}
.post-tags {
  margin-bottom: 10px;
}
.post-tags .tag {
  display: inline-block;
  background-color: #f0f0f0;
  color: #666;
  padding: 2px 6px;
  border-radius: 3px;
  margin-right: 8px;
  font-size: 12px;
}
.post-ops {
  display: flex;
  font-size: 12px;
  color: #888;
}
.post-ops span {
  margin-right: 15px;
  cursor: pointer;
}
/* //.page-count居中对齐 */
.page-count {
  margin-top: 20px;
  text-align: center;
  justify-content: center;
}
</style>