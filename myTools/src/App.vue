<script setup lang="ts">
const imgs = [
  'Weixin Image_20231222090523.jpg',
  'Weixin Image_20231222090756.jpg',
  'Weixin Image_20231222090903.jpg',
  'Weixin Image_20231222091407.jpg'
]
</script>

<template>
  <div class="flex mt-0">
    <el-carousel class="w-1600px h-600px mt-0px">
      <el-carousel-item v-for="item in imgs" :key="item">
        {{ item }}
        <el-image :src="'./assets/imgs/' + item" fit="fill"></el-image>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<style scoped></style>
