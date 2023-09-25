<template>
  <div style="margin-top: 0px;">
<<<<<<< HEAD
    <!-- <navbarLogin msg="Plaese Login before Use"/> -->
  </div>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/HandLogo.png"> -->
  </div>
  <div style="margin-top: -10px;">
=======
    <navbarLogin msg="Plaese Login before Use"/>
  </div>
  <div class="home">
    <img alt="Vue logo" src="../assets/HandLogo.webp">
  </div>
  <div style="margin-top: 20px;">
>>>>>>> 58b60b900071cf6160f9cecee99de9cc964959ac
    <LoginPage msg="Plaese Login before Use"/>
  </div>
</template>

<script>
// @ is an alias to /src
import LoginPage from '@/components/Login.vue'
<<<<<<< HEAD
// import navbarLogin from '@/components/navbarLogin.vue'
=======
import navbarLogin from '@/components/navbarLogin.vue'
>>>>>>> 58b60b900071cf6160f9cecee99de9cc964959ac

export default {
  name: 'HomeView',
  components: {
    LoginPage,
<<<<<<< HEAD
    // navbarLogin
=======
    navbarLogin
>>>>>>> 58b60b900071cf6160f9cecee99de9cc964959ac
  }
}
</script>
<style scoped>
.home{
  text-align: center;
}
img {
  max-width: 50%; /* ขยายภาพให้เต็มขนาดของพื้นที่ */
  height: 150px; /* ปรับสูงตามอัตราส่วน */
  margin: 0 auto; /* จัดตรงกลางแนวนอน */
  display: block; /* จัดให้อยู่ตรงกลางแนวนอน */
}
</style>
