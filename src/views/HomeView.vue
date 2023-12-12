<template>
  <div class="home">
    <HomeCarousel></HomeCarousel>
    <HomeWelcome></HomeWelcome>
  </div>
</template>

<script setup>
import HomeWelcome from '../components/home/HomeWelcome.vue'
import HomeCarousel from '../components/home/HomeCarousel.vue'
</script>

<style>
body {
  padding: 0;
  margin: 0;
}

html,
body {
  text-align: center;
}

.home-logo {
  padding-top: 40px;
  padding-bottom: 40px;
  height: 80px;
}

.home {

}
</style>
