<template>
  <div class="m-login-wrap">
    <div class="m-login-row">
      <input type="text" class="m-login-input" placeholder="请入手机号码" v-model="username" />
    </div>
    <div class="m-login-row">
      <input type="password" class="m-login-input" placeholder="请入密码密码" v-model="password" />
    </div>
    <div class="m-login-row">
      <button class="m-login-btn" @click="handleLogin">登陆</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      username: '',
      password: ''
    }
  },
  methods: {
    handleLogin() {
      let temp = {
        phone: this.username,
        password: this.password
      }
      console.log(temp)
    }
  }
}
</script>

<style scoped>
.m-login-wrap{margin:0 20px;}
.m-login-row{margin:20px;}
.m-login-input{display:block;width:100%;height:40px;}
.m-login-btn{display:block; width:100%;height:40px;border-radius:20px;}
</style>
