<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****2211 完成了 100 万字克苏鲁赛博朋克大纲规划"
  },
  {
    "text": "用户 189****9900 获得了凡人流仙侠前三章黄金钩子细纲"
  },
  {
    "text": "用户 131****4455 完成了都市神医马甲流人设与反派矩阵"
  },
  {
    "text": "用户 156****7788 生成了悬疑推理小说九重迷局分卷大纲"
  },
  {
    "text": "用户 173****3311 取得了网文签约拆解与黄金前三章防毒指南"
  }
]);
</script>
