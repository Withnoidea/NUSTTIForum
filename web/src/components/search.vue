<template>
  <el-input
    v-model="input"
    style="width: 240px"
    placeholder="搜索帖子 / 活动 / 用户..."
    clearable
  />
</template>

<script lang="ts" setup>
import { ref } from 'vue'

const input = ref('')
</script>
