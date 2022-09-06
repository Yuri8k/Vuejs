<template>
  <div id="nav">
    <router-link to="/">
        <img :src="logo" :alt="alt" id="logo">
    </router-link>
    <div>
      <router-link to="/">Home</router-link> 
      <router-link to="/pedidos">Pedidos</router-link>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Navbar',
    props: ['logo', 'alt']
}
</script>

<style scoped>
  #nav {
    background: #222;
    border-bottom: 4px solid #111;
    padding: 15px 50px;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  #nav a {
    color: #fcba03;
    text-decoration: none;
    margin: 12px;
    transition: .5s ease;
  }

  #nav a:hover {
    color: #fff;
    transition: .5s ease
  }

  #logo {
    width: 100%;
    display: block;
    max-width: 40px;
  }
</style>

