<template>
  <div class="login-view">
    <div class="login-form">
      <h1 class="login-title">Login</h1>
      <input v-model="username" placeholder="Username" @keyup.enter="login">
      <input v-model="password" type="password" placeholder="Password" @keyup.enter="login">
      <button @click="login">Login</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      username: '',
      password: ''
    };
  },
  methods: {
    login() {
      if (this.username === 'admin' && this.password === 'admin123') {
        this.$router.push('/home');
      } else {
        alert('Invalid credentials');
      }
    }
  }
};
</script>

<style>
.login-view {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.login-form {
  text-align: center;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 5px;
  background-color: #f9f9f9;
  box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.1);
}

.login-title {
  margin-bottom: 10px;
  font-size: 24px;
  font-weight: bold;
}
</style>
