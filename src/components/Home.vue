<template>
    <div class="home-container">
      <h1>Welcome to Home Page</h1>
      <!-- โค้ดเนื้อหาหน้า Home อื่น ๆ ของคุณ -->
    </div>
  </template>
  
  <script>
  export default {
    name: 'HomePage', // ระบุชื่อของคอมโพเนนต์เป็น "Home"
    // สามารถเพิ่มโค้ดของคอมโพเนนต์ Home อื่น ๆ ตามต้องการ
  };
  </script>
  
  <style scoped>
  /* สไตล์ของ Home.vue */
  .home-container {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
  }
  
  h1 {
    font-size: 24px;
    text-align: center;
  }
  </style>
  