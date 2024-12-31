<template>
<div id="nav">
    <router-link to="/" id="logo-url">
        <img id="logo" :src="logo" :alt="alt">
    </router-link>
    <h1 id="rest-name">DELICIOUS <span style="color: #FFF;">DOG</span></h1>
    <nav>
        <router-link to="/">Home</router-link>
        <router-link to="/pedidos">Orders</router-link>
    </nav>
</div>
</template>

<script>
export default {
    name: "Navbar",
    props: ["logo", "alt"]
}
</script>

<style scoped>
#nav {
    background-color: #222;
    border-bottom: 4px solid #111;
    padding: 15px 50px;
    display: flex;
    justify-content: space-between; /* Distribui espaço entre os elementos */
    align-items: center;
}

#rest-name {
    color: #fcba03;
    font-size: 1.5rem;
    margin: 0 auto; /* Centraliza o texto dentro da Navbar */
    text-align: center;
}

#logo-url {
    margin-right: 20px; /* Ajuste opcional para espaçamento do logo */
}

#logo {
    width: 40px;
    height: 40px;
}

#nav a {
    color: #fcba03;
    text-decoration: none;
    margin: 12px;
    transition: 0.5s;
}

#nav a:hover {
    color: #FFF;
}
</style>