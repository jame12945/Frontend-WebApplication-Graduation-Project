<template>
    <nav id="navhome">
     <li class="HomeLink"><router-link to="/HomeComponent">Home</router-link></li>
     <li class="HomeLink"><router-link to="/HomeComponent">Room</router-link></li>
     <li class="HomeLink"><router-link to="/HomeComponent">Calendar</router-link></li>
     <li class="HomeLink"><router-link to="/HomeComponent">About</router-link></li>
     <li class="HomeLink"><router-link to="/HomeComponent">Help</router-link></li>

    </nav>
</template>
<script>

export default {
  name: 'navHome',
  }

</script>
<style scoped>
.HomeLink a{
    color: rgb(255, 255, 255);
}

li a:hover {
  color: rgb(234, 190, 136);
  transition: 0.5s;
}
nav {
    border-bottom: none;
    background: none;
}


</style>