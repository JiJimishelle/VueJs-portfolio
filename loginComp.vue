<template>
  <div class="wrapper">
    <h1>로그인</h1>
    <form id="login-form" @submit.prevent="handleLogin">
      <div class="input-box">
        <input type="text" id="username" v-model="username" name="username" placeholder="아이디" required>
        <i class='bx bxs-user'></i>
      </div>
      <div class="input-box">
        <input type="password" id="password" v-model="password" name="password" placeholder="비밀번호" required>
        <i class='bx bxs-lock-alt'></i>
      </div>
      <div class="remember-forgot">
        <input type="checkbox" id="remember-me">
        <label for="remember-me">로그인 상태 유지</label>
      </div>
      <button type="submit" class="btn">로그인</button>
    </form>
  </div>
</template>

<script>
export default {
  name: 'LoginComp',
  data() {
    return {
      username: '',
      password: ''
    };
  },
  methods: {
    handleLogin() {
      if (this.username === '202339186' && this.password === '20040601') {
        alert('로그인되었습니다.');
      } else {
        alert('회원정보가 있지 않습니다.');
      }
    }
  }
};
</script>

<style scoped>
  .wrapper {
      width: 400px;
      align-items: center;
      margin: 10% auto;
      padding: 40px 30px;
      border-radius: 10px;
      box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.1);
      text-align: center;
  }
  .wrapper h1 {
      font-size: 24px;
      margin-bottom: 20px;
  }
  .input-box {
      position: relative;
      margin-bottom: 30px;
  }
  .input-box input {
      width: 100%;
      height: 45px;
      background: transparent;
      border: 2px solid black;
      border-radius: 25px;
      font-size: 16px;
      color: #fff;
      padding: 0 15px 0 45px;
      box-sizing: border-box;
      transition: border 0.3s ease;
  }
  .input-box input:focus {
      border-color: #080808;
  }
  .input-box input::placeholder {
      color: black;
  }
  .input-box i {
      position: absolute;
      top: 50%;
      left: 15px;
      transform: translateY(-50%);
      font-size: 18px;
      color: black;
  }
  .remember-forgot {
      display: flex;
      align-items: center;
      margin-bottom: 20px;
      font-size: 14px;
  }

  .btn {
      width: 100%;
      height: 45px;
      background-color: #080808;
      color: #fff;
      border: none;
      border-radius: 25px;
      font-size: 18px;
      cursor: pointer;
      transition: background-color 0.3s ease;
  }
  .btn:hover {
      background-color: #000;
  }
</style>
