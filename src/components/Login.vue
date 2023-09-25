<template>
<<<<<<< HEAD
  <div class="image-container">
    <h1 style=" margin-top: -520px;width:200px;color: rgb(255, 255, 255);font-size: 40px;">WEBSITE NAME</h1>
  </div>
  <div class="login-container">
    
    <h1 style="text-align: center; font-size: 24px; margin-bottom: 25px; margin-top: 40px;margin-left:20px">LOGIN</h1>
    <form @submit.prevent="login">
      <div class="form-group">
        <label for="username" style="font-size: 20px;">Username</label>
        <input type="text" id="username" style="text-align: center; background-color: black; color: white;" v-model="username" required>
      </div>
      <div class="form-group">
        <label for="password" style="font-size: 20px;">Password</label>
        <input type="password" id="password" style="text-align: center;" v-model="password" required>
=======
  <div class="login-container">
    <h1 style="text-align: center; font-size: 20px; margin-bottom: 25px; margin-top: 15px;">LOGIN</h1>
    <form @submit.prevent="login">
      <div class="form-group">
        <label for="username">Username</label>
        <input type="text" id="username" v-model="username" required>
      </div>
      <div class="form-group">
        <label for="password">Password</label>
        <input type="password" id="password" v-model="password" required>
>>>>>>> 58b60b900071cf6160f9cecee99de9cc964959ac
      </div>
      <button type="submit">Submit</button>
      <div class="click">Dont have account? <router-link to="/Register" class="here">Click here</router-link></div>
    </form>
  </div>
</template>

<script>
export default {
  name: 'LoginForm', // ระบุชื่อของคอมโพเนนต์เป็น "LoginForm"
  data() {
    return {
      username: '',
      password: ''
    };
  },
  methods: {
    login() {
      // ในส่วนนี้คุณสามารถทำการตรวจสอบการเข้าสู่ระบบของผู้ใช้
      // โดยตรวจสอบ username และ password จากข้อมูลในฐานข้อมูลหรือระบบของคุณ
      // และทำการเปลี่ยนเส้นทางหรือดำเนินการที่เหมาะสมตามผลลัพธ์

      if (this.username === 'example' && this.password === 'password') {
        // สำเร็จ: เข้าสู่ระบบและทำการเปลี่ยนเส้นทางไปยังหน้าอื่น
        this.$router.push('/HomeComponent'); // ตัวอย่างการเปลี่ยนเส้นทางไปยังหน้า dashboard
      } else {
        // ไม่สำเร็จ: แสดงข้อความผิดพลาดหรือทำอย่างอื่นตามต้องการ
        alert('Login failed. Please check your credentials.');
      }
    }
  }
};
</script>

<style scoped>

.login-container {
<<<<<<< HEAD
  width: 450px;
  height: 480px;
  margin: 0 auto;
  padding-right: 15px;
  border-radius: 10px;
  background-color: rgba(195, 195, 195, 0.7);
  display: flex;
  flex-direction: column;
  align-items: center;
  position: absolute;
  top: 60%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: 1;
}

.image-container {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 814px;
  background: url(../assets/firstPagePic.png) no-repeat center center;
  background-size: cover;
  overflow: hidden;
  
}

.form-group {
  margin-bottom: 22px;
=======
  max-width: 320px;
  margin: 0 auto;
  padding: 10px;
  border-radius: 10px;
  background-color: rgba(255, 255, 255, 0.7);
}

.form-group {
  margin-bottom: 15px;
>>>>>>> 58b60b900071cf6160f9cecee99de9cc964959ac
  
}
.click {
  margin-bottom: 25px;
  margin-top: 20px;
  text-align: center;
<<<<<<< HEAD
  font-size: 18px;
}
.here{
  text-decoration: underline;
  color: #885B3B;
}
.here:hover{
  color: rgb(208, 111, 0);
=======
}
.here{
  text-decoration: underline;
  color: red;
}
.here:hover{
  color: blue;
>>>>>>> 58b60b900071cf6160f9cecee99de9cc964959ac
  transition: 0.5s;
}
label {
  display: block;
  margin-bottom: 5px;
  text-align: left;
  margin-left: 17px;
  font-weight: bold;
}

input {
<<<<<<< HEAD
  width: 350px;
  height: 30px;
  padding: 5px 0px;
  border: none;
  border-radius: 10px;
  position: relative;
  padding-left: 5px;
  background-color: black; /* ตั้งค่าพื้นหลังเป็นสีดำ */
  color: white; /* ตั้งค่าสีข้อความเป็นสีขาว */
=======
  width: 280px;
  height: 25px;
  padding: 5px 0px;
  border: 1.5px solid #885B3B;
  border-radius: 5px;
  position: relative;
  padding-left: 5px;
  background-color: rgba(255, 255, 255, 0.7);
  color: #000000;
>>>>>>> 58b60b900071cf6160f9cecee99de9cc964959ac
  margin-left: 17px;
}

button {
  background-color: #885B3B;
  color: #fff;
  padding: 10px 15px;
<<<<<<< HEAD
  height: 42px;
  border: none;
  border-radius: 10px;
  width: 350px;
=======
  border: 1.5px solid #ffffff;
  border-radius: 5px;
  width: 288px;
>>>>>>> 58b60b900071cf6160f9cecee99de9cc964959ac
  cursor: pointer;
  font-weight: bold;
  font-family: serif;
  margin-left: 15px;
<<<<<<< HEAD
  margin-top: 0px;
  font-size: 18px;
}
/* 
button:hover{
  background-color:#181818;
  border: none;
  color: #ffffff;
  
} */
=======
  margin-top: 15px;
}

button:hover{
  background-color:#ffffff;
  border: 1.5px solid #885B3B;
  color: #885B3B;
  transition: 0.3s;
}
>>>>>>> 58b60b900071cf6160f9cecee99de9cc964959ac

</style>
