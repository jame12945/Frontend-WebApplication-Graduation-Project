<template>
  <div style="margin-top: 0px;">
    <!-- <navbarLogin msg="Plaese Login before Use"/> -->
  </div>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/HandLogo.png"> -->
  </div>
  <div style="margin-top: -10px;">
    <LoginPage msg="Plaese Login before Use"/>
  </div>
</template>

<script>
// @ is an alias to /src
import LoginPage from '@/components/Login.vue'
// import navbarLogin from '@/components/navbarLogin.vue'

export default {
  name: 'HomeView',
  components: {
    LoginPage,
    // navbarLogin
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
