<template>
    <nav id="nav">
      <li><router-link to="/" style="background-color: rgb(255, 255, 255); font-size: 20px; font-weight: bold;">Kongtel</router-link></li>
      <li><router-link to="/about">Properties</router-link></li>
      <li><router-link to="/profile">Reviews</router-link></li>
      <li><router-link to="/profile">Populars</router-link></li>
      <li class="Login-button"><router-link to="/Login">Login</router-link></li>
      <li class="Sign-button"><router-link to="/Register">Sign-up</router-link></li>
      
    </nav>
    <router-view/>
  </template>

<style>
.Sign-button {
  float: right;
}
.Sign-button a{
  border-radius: 10px; 
  background-color: #ffffff;
  border: 1px solid #8E5F34;
  color: #8E5F34;
}
.Login-button {
  float: right;
  padding-right: 20px;
}
.Login-button a{
  border-radius: 10px; 
  background-color: #8E5F34;
  border: 1px solid #8E5F34;
  color: #ffffff;
}
.Login-button a:hover{
  background-color: #ffffff;
  color: #8E5F34;
  border: 1px solid #8E5F34;
  transition: 0.5s;
}
.Sign-button a:hover{
  background-color: #8E5F34;
  color: #ffffff;
  border: 1px solid #8E5F34;
  transition: 0.5s;
}
nav {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #ffffff;
  border-bottom: 2px solid #C5BDBD;
  
}
li {
  float: left;
  margin-top: 5px;
  margin-bottom: 10px;
  padding-left: 10px;
  
}


li a {
  display: block;
  color: #8E8282;
  text-align: center;
  padding: 10px 44px;
  text-decoration: none;
}
li a:hover {
  color: #111;
  transition: 0.5s;
}

nav a.router-link-exact-active {
  color: #8E5F34;
}
</style>