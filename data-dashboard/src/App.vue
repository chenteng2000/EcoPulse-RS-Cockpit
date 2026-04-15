<script setup lang="ts">
import { onMounted, ref } from 'vue';
import { Viewer, Ion } from 'cesium';

// 注意：如果你有 Cesium Ion 的 Token，可以填在这里，否则会使用默认的底图（有配额限制）
// Ion.defaultAccessToken = 'YOUR_CESIUM_ION_TOKEN_HERE';

const viewerRef = ref<HTMLDivElement | null>(null);

onMounted(() => {
  if (viewerRef.value) {
    new Viewer(viewerRef.value, {
      animation: false,       // 隐藏底部动画控制条
      timeline: false,        // 隐藏底部时间线
      infoBox: false,         // 隐藏点击弹窗
      geocoder: false,        // 隐藏地理编码搜索框
      baseLayerPicker: false, // 隐藏底图切换器
    });
  }
});
</script>

<template>
  <!-- 使用 Tailwind CSS 类名：全屏、背景黑色、无滚动条 -->
  <div ref="viewerRef" class="w-screen h-screen bg-black m-0 p-0 overflow-hidden"></div>
</template>