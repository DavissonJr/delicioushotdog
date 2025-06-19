<template>
  <div id="main-banner">
    <h1>ME DÊ O SEU MELHOR!</h1>
  </div>
</template>

<script>
import BurgerForm from '@/components/BurgerForm.vue';

export default {
  name: "Banner",
  components: {
    BurgerForm
  }
}
</script>

<style scoped>
#main-banner {
  height: 100vh; 
  max-height: 700px; 
  background-image: url("/public/img/hotdog.jpg");
  background-position: center; 
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}

#main-banner h1 {
  color: #FFF;
  text-align: center;
  font-size: 4rem;
  padding: 20px 40px;
  border: 2px solid white;
  border-radius: 2rem;
  margin-left: 3rem;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.5);
}

@media (max-width: 768px) {
  #main-banner {
    height: 600px;
  }

  #main-banner h1 {
    font-size: 2.5rem; 
    padding: 10px 20px; 
  }
}
</style>