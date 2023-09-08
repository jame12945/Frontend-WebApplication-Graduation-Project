<template>
    <div class="Register-container">
      <h1 style="text-align: center;">Register</h1>
      <form @submit.prevent="Register">
        <div class="Rform-group">
          <label for="username">Username</label>
          <input type="text" id="username" v-model="username" required>
        </div>
        <div class="Rform-group">
          <label for="password">Password</label>
          <input type="password" id="password" v-model="password" required>
        </div>
        <button type="submit">Register</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    name: 'RegisterForm', // ระบุชื่อของคอมโพเนนต์เป็น "LoginForm"
    data() {
      return {
        username: '',
        password: ''
      };
    },
    methods: {
        Register() {
        // ในส่วนนี้คุณสามารถทำการตรวจสอบการเข้าสู่ระบบของผู้ใช้
        // โดยตรวจสอบ username และ password จากข้อมูลในฐานข้อมูลหรือระบบของคุณ
        // และทำการเปลี่ยนเส้นทางหรือดำเนินการที่เหมาะสมตามผลลัพธ์
  
        if (this.username === 'example' && this.password === 'password') {
          // สำเร็จ: เข้าสู่ระบบและทำการเปลี่ยนเส้นทางไปยังหน้าอื่น
          this.$router.push('/HomeComponent'); // ตัวอย่างการเปลี่ยนเส้นทางไปยังหน้า dashboard
        } else {
          // ไม่สำเร็จ: แสดงข้อความผิดพลาดหรือทำอย่างอื่นตามต้องการ
          alert('Register failed. Please check your credentials.');
        }
      }
    }
  };
  </script>
  
  <style scoped>
  
  .Register-container {
    max-width: 400px;
    margin: 0 auto;
    padding: 10px;
    border: 2px solid #6a6a6a;
    border-radius: 5px;
    background-color: rgba(0, 0, 0, 0.15);
  }
  
  .Rform-group {
    margin-bottom: 15px;
  }
  
  label {
    display: block;
    margin-bottom: 5px;
    
    
  }
  
  input {
    width: 90%;
    height: 25px;
    padding: 0px;
    border: 2px solid #afafaf;
    border-radius: 3px;
    position: relative;
    padding-left: 5px;
  }
  
  button {
    background-color: #000000;
    color: #fff;
    padding: 8px 15px;
    border: 2px solid #ffffff;
    border-radius: 3px;
    cursor: pointer;
    
  }
  
  button:hover{
    background-color:#ffffff;
    border: 2px solid #000000;
    color: #000000;
    transition: 0.3s;
  }
  
  </style>