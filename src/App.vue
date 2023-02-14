<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/pagination';
import 'swiper/css/navigation';

// import required modules
import { Autoplay, Pagination, Navigation } from 'swiper';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Autoplay, Pagination, Navigation],
    };
  },
};
</script>

<template>
<div class="container">
  <div class="header">
    <div class="logo"><img src="./assets/Blue.svg"></div>
    <div class="menu">
      <ul>
        <li><a href="#">home</a ></li>
        <li><a href="#">aboutus</a ></li>
        <li><a href="#">contact</a ></li>
      </ul>
    </div>
    <div class="login">
      <a href="#">login</a>
    </div>
  </div>
  <div class="banner">

    <swiper
        :autoplay="{
          delay: 2500,
          disableOnInteraction: false,
        }"
        :pagination="{
          clickable: true,
        }"
        :navigation="true"
        :modules="modules"
        class="mySwiper"
        :style="{
           '--swiper-navigation-color': '#fff',
          '--swiper-pagination-color': '#fff',
        }">
          <swiper-slide><img src="./assets/Bitmap.png" alt="img"></swiper-slide>
          <swiper-slide><img src="./assets/Bitmap.png" alt="img"></swiper-slide>
          <swiper-slide><img src="./assets/Bitmap.png" alt="img"></swiper-slide>
    </swiper>
  </div>
</div>
</template>

<style scoped>
.container{
  width: 100%;
  height: 100px;

}
.header {
  width: 1200px;
  height: 100px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}
.logo {
  width: 200px;
  height: 100%;
  display: flex;
  align-items: center;
}
.logo img {
  height:30px;
}
.menu {
  flex: 1;
  height: 100%;
}
.menu ul {
  display: flex;
  justify-content: center;
}
.menu li {
  list-style: none;
  width: 100px;
  line-height: 100px;
  color: #181818;
  font-size: 14px;
  text-transform: uppercase;

}
.menu a:link {
  color: #2c3e50;
  text-decoration: none;
  font-weight: bold;
}
.menu a:visited {
  color: #2c3e50;
  text-decoration: none;
  font-weight: bold;
}
.menu a:hover {
  color: aqua;
  text-decoration: none;
  font-weight: bold;
}
.menu a:active {
  color: aqua;
  text-decoration: none;
  font-weight: bold;
}
.login{
  width: 200px;
  height: 100px;
  display: flex;
  align-items: center;
}
.login a {
  width: 200px;
  height: 50px;
  border-radius: 5px;
  background-color: #2c3e50;
  font-size: 14px;
  color: #f2f2f2;
  text-align: center;
  line-height: 50px;
  font-weight: bold;
  text-decoration: none;
}
.login a:link{
  background-color: #2c3e50;
}
.login a:visited {
  background-color: #2c3e50;
}
.login a:hover {
  background-color: aqua;
}
.banner img {
  width: 100%;
  height: 560px;
  object-fit: cover;
}
</style>
