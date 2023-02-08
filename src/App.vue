<script setup>
</script>

<template>
  <div class="header">
    <div class="main_1200">
      <div class="top_logo"><img src="./assets/Blue.svg"></div>
      <div class="top_menu">
        <ul>
          <li><a href="#">Worlk</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </div>
      <div class="login">
        <button>login</button>
      </div>
    </div>
  </div>
  
  <div class="banner">
    <div><img src="../src/assets/Bitmap.png"></div>
  </div>
</template>

<style scoped>
.header {
  width: 100%;
  height: 100px;
  background-color: #ffffff;
  text-align: center;

}
.main_1200{
  width: 1200px;
  height: 100px;
  margin: auto;
}
.top_logo{
  float: left;
  vertical-align:middle ;
  padding-top: 30px;

}
.header .top_logo img {
  width: 123px;
  height: 40px;
}
.top_menu {
  width: 600px;
  height: 100px;
  float: left;
  padding-left: 300px;
  list-style-type: none;

  }
.top_menu li {
  list-style-type: none;
  float: left;
  font-size: 14px;
  color: #333333;
  width: 100px;
  line-height: 100px;
  font-weight: bold;
}
.top_menu a:link {
  text-decoration: none;
  font-size: 14px;
  color: #333333;
  font-weight: bold;
}
.top_menu a:visited {
  text-decoration: none;
  font-size: 14px;
  color: #333333;
  font-weight: bold;
}
.top_menu a:hover {
  color: #134DAB;
}
.top_menu a:active {
  color: #134DAB;
}
.login {
  width: 200px;
  float:right;
  padding-top: 23px;
}
.login button {
  width: 200px;
  height: 50px;
  background-color:#134DAB;
  color: #ffffff;
  border-radius: 5px;
  font-size: 16px;
  font-weight: bold;
  border-style: none;

}
</style>
