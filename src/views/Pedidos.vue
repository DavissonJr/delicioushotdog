<template>
  <div class="main-container">
    <h1>Manage Orders:</h1>
    <Dashboard/>  
  </div>
</template>

<script>
import Dashboard from '@/components/Dashboard.vue';

export default{
  name: "Pedidos",
  components:{
    Dashboard
  }
}
</script>

<style scoped>
h1{
  margin-top: 2rem;
  margin-bottom: -.5rem;
}

</style>
