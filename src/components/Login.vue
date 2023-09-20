<template>
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
  max-width: 320px;
  margin: 0 auto;
  padding: 10px;
  border-radius: 10px;
  background-color: rgba(255, 255, 255, 0.7);
}

.form-group {
  margin-bottom: 15px;
  
}
.click {
  margin-bottom: 25px;
  margin-top: 20px;
  text-align: center;
}
.here{
  text-decoration: underline;
  color: red;
}
.here:hover{
  color: blue;
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
  width: 280px;
  height: 25px;
  padding: 5px 0px;
  border: 1.5px solid #885B3B;
  border-radius: 5px;
  position: relative;
  padding-left: 5px;
  background-color: rgba(255, 255, 255, 0.7);
  color: #000000;
  margin-left: 17px;
}

button {
  background-color: #885B3B;
  color: #fff;
  padding: 10px 15px;
  border: 1.5px solid #ffffff;
  border-radius: 5px;
  width: 288px;
  cursor: pointer;
  font-weight: bold;
  font-family: serif;
  margin-left: 15px;
  margin-top: 15px;
}

button:hover{
  background-color:#ffffff;
  border: 1.5px solid #885B3B;
  color: #885B3B;
  transition: 0.3s;
}

</style>
