<template>
  <div>
    <Banner />
    <div class="main-container">
      <h1>MAKE YOUR HOTDOG!</h1>
      <BurgerForm />
    </div>
  </div>
</template>

<script>
import Banner from '../components/Banner'
import BurgerForm from '../components/BurgerForm'

export default {
  name: 'Home',
  components: {
    Banner,
    BurgerForm
  }
}
</script>

<style scoped>
h1{
  margin-top: 0.5rem;
}
</style>