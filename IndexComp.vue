<template>
  <div class="profile-container">
    <img src="../assets/profile.png" alt="나의 사진!!!" class="profile-image" />
    <div class="text-overlay">
      <p>가천대학교 IT융합대학 컴퓨터공학전공 2학년 학생</p>
      <br>
      <h1>안녕하십니까,<br>몽골에서 온 미실입니다.</h1>
      <br>
      <button class="login-button" @click="goToLogin">로그인</button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    goToLogin(){
      this.$router.push({ name: 'LoginComp' });
    }
  }
};
</script>


<style scoped>
p{
  color: white;
}
.profile-container {
  position: relative;
  max-width: 500px;
}

.profile-image {
  display: block;
}

.text-overlay {
  position: absolute;
  top: 25%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: justify;
  width: 100%;
}

.text-overlay p, .text-overlay h1 {
  margin: 0;
  padding: 0;
}

.login-button {
  display: block;
  margin-top: 20px;
  padding: 10px 20px;
  font-size: 16px;
  color: white;
  background-color: black;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.login-button:hover {
  background-color: white;
  color: black;
}
</style>
