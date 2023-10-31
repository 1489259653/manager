<template>
  <div class="login-container">

      <div class="title-container">
        <h3 class="title">用户登录</h3>
      </div>
      <el-form-item>
        <el-icon><User /></el-icon>
        <el-input ></el-input>
      </el-form-item>
      <el-form-item >
        <el-icon><Lock /></el-icon>
        <el-input v-model="loginForm.password" :type="passwordType"></el-input>
      </el-form-item>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { User, Lock } from '@element-plus/icons-vue'
const loginForm = ref({
  username: 'admin',
  password: '123456'
})

</script>

<style lang="scss" scoped>

</style>
