<template>
  <img alt="Vue logo" src="../assets/tdw logo.png">
    <div>
      <h3 class="login-email-input login-input">email</h3>
      <input type="text" placeholder="Enter Email" class="login-input-field" required>
      <h3 class="login-pw-input login-input">password</h3>
      <input type="text" placeholder="Enter Password" class="login-input-field" required>
    </div>
    <div>
      <button class="login-button" @click="handleLogin">로그인</button>
    </div>
    <div>
      <button class="signup-button" @click="goToSignUp">회원가입</button>
    </div>
    
  </template>
  
<script>
import '@/assets/css/Login.css';

export default {
  name: 'LoginPage',
  methods: {
    goToSignUp() {
      this.$router.push('/signup'); // 회원가입 페이지로 이동
    }
  }
}
</script>