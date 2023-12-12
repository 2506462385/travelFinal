<script setup>
import {ref} from "vue";

const images = ref([
  'src/assets/banner1.jpeg',
  'src/assets/banner2.jpeg',
  'src/assets/banner3.jpeg',
  'src/assets/banner4.jpeg',
  'src/assets/banner5.jpeg',
  'src/assets/banner6.jpeg']
)
</script>

<template>

  <el-carousel :interval="4000" type="card" height="200px">
    <el-carousel-item v-for="item in images" :key="item">
      <img :src="item" class="banner-img" alt="无法加载图片">
    </el-carousel-item>
  </el-carousel>

</template>

<style>
.banner-img {
  width: 100%;
  position: relative;
  bottom: 50px;
}

.el-carousel__item h3 {
  color: #475669;
  opacity: 0.75;
  line-height: 200px;
  margin: 0;
  text-align: center;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}

</style>
