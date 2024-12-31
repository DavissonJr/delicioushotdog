<template>
  <div>
    <Navbar :logo="logo_src" :alt="app_name" />
    <div>
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import Navbar from './components/Navbar'

export default {
  data: function() {
    return {
      logo_src: "/img/logo.png",
      app_name: "Make Your HotDog"
    }
  },
  components: {
    Navbar,
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Funnel+Display:wght@300..800&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700&family=Quicksand:wght@300..700&family=Sour+Gummy:ital,wght@0,100..900;1,100..900&family=Ubuntu+Condensed&family=Ubuntu:ital,wght@0,300;0,400;0,500;0,700;1,300;1,400;1,500;1,700&display=swap');

* {
  font-family: "Poppins", serif;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.main-container {
  display: flex; 
  flex-direction: column; 
  height: 70dvh;
}

h1 {
  text-align: center;
  font-size: 2.5rem;
  margin-bottom: 30px;
  color: #222;
}
</style>
