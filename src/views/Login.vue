<template>
  <div>
      <el-form ref="form" :model="loginForm">
        <h3>系统登录</h3>
        <el-form-item>
          <el-input type="text" auto-complete="false" v-model="loginForm.username" placeholder="请输入用户名">
          </el-input>
        </el-form-item>
        <el-form-item>
          <el-input type="password" auto-complete="false" v-model="loginForm.password" placeholder="请输入密码">
          </el-input>
        </el-form-item>
        <el-form-item>
          <el-input type="text" auto-complete="false" v-model="loginForm.code" placeholder="点击更换图片">
          </el-input>
          <img src="">
          <el-checkbox v-model="checked">记住我</el-checkbox>
          <el-button type="primary">登录</el-button>
        </el-form-item>
      </el-form>

  </div>

</template>

<script>
export default {
  name: "Login",
  data(){
    return{
      loginForm:{
        username : 'admin',
        password : '123',
        code: ''
      }
    }
  }
}
</script>

<style scoped>

</style>