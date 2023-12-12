<script setup>
import {RouterLink, RouterView} from 'vue-router'
import HomeView from './views/HomeView.vue'
import LoginView from "@/views/LoginView.vue";

</script>

<template>
  <div class="app">
    <RouterLink to="/login">login</RouterLink>
    <RouterView style="padding-top: 60px"/>
  </div>
</template>

<style>
.nav-bar {
  position: center;
  z-index: 10;
  width: 100%;
}

el-menu-item {
  height: 30px;
}

.personal-wrapper {
  text-align: center;
}

.personal-item {
  cursor: pointer;
  line-height: 40px;
}

.personal-item :hover {
  background-color: #aaaaaa;
}

.header-logo {
  height: 50px;
  position: fixed;
  left: 10px;
  top: 5px;
  z-index: 10;
}

.login-icon {
  z-index: 1;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  border: solid 2px lightgray;
  cursor: pointer;
}

.header-user {
  position: fixed;
  right: 30px;
  top: 10px;
  height: 50px;
  line-height: 50px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  border-bottom: solid 0.5px #42b983;
  background-color: white;
  padding: 20px;
  position: fixed;
  width: 100%;
  top: 0;
  text-align: center;
}

a {
  font-weight: normal;
  color: #2c3e50;
  text-decoration: none;
  margin-left: 80px;
}


</style>
