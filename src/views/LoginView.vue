<script setup>
import {ref} from "vue";
const user = ref({
  userName:'',
  password:''
})

const rules = {
  username:[{
    required:true,
    message:'账号不可为空',
    trigger:'blur'
  }],
  password:[{
    required:true,
    message:'密码不可为空',
    trigger:'blur'
  }]
}
</script>
<template>

  <div class="main">
      <el-form  :rules="rules" label-width="80px" class="login-box">
        <h3 class="login-title">欢迎登录</h3>
        <el-form-item label="用户名" prop="userName">
          <el-input type="text" placeholder="请输入账号" v-model="user.userName"/>
        </el-form-item>
        <el-form-item label="密码" prop="userPassword">
          <el-input type="password" placeholder="请输入密码" v-model="user.password"/>
        </el-form-item>
        <el-form-item>
          <el-button type="primary" v-on:click="onLogin('loginForm')">登录</el-button>
          <el-button type="primary" class="register-button" v-on:click="onRegist()">注册新用户</el-button>
        </el-form-item>
      </el-form>
    </div>
<!--    <div v-else>-->
<!--      <el-form ref="registerForm" :model="registerForm" :rules="registerRules" label-width="80px"-->
<!--               class="login-box">-->
<!--        <h3 class="login-title">注册新用户</h3>-->
<!--        <el-form-item label="姓名" prop="userName">-->
<!--          <el-input v-model="registerForm.userName"></el-input>-->
<!--        </el-form-item>-->
<!--        <el-form-item label="密码" prop="userPassword">-->
<!--          <el-input v-model="registerForm.userPassword" show-password></el-input>-->
<!--        </el-form-item>-->
<!--        <el-form-item label="年龄" prop="userAge">-->
<!--          <el-input v-model="registerForm.userAge"></el-input>-->
<!--        </el-form-item>-->
<!--        <el-form-item label="性别" prop="userSex">-->
<!--          <el-input v-model="registerForm.userSex"></el-input>-->
<!--        </el-form-item>-->
<!--        <el-form-item label="电话" prop="userSex">-->
<!--          <el-input v-model="registerForm.userPhone"></el-input>-->
<!--        </el-form-item>-->
<!--        <el-form-item>-->
<!--          <el-button type="primary" @click="onSubmitRegist('registerForm')">注 册</el-button>-->
<!--          <el-button @click="onCancelRegist()">取 消</el-button>-->
<!--        </el-form-item>-->
<!--      </el-form>-->
<!--    </div>-->

</template>

<style scoped>

</style>
