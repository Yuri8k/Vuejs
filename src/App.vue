<template>
  <div>
      <NavbarVue :logo="logo_scr" :alt="app_name"/> 
      <router-view/>
      <Footer />
  </div>
</template>

<script>
import NavbarVue from './components/Navbar.vue';
import Footer from './components/Footer.vue';

export default {
  name: '#App',
  components: {
    NavbarVue,
    Footer
  },
  data() {
    return {
      logo_scr: "/img/logo.png",
      app_name: "logo"
    }
  }
}
</script>

<style>
  * {
    font-family: Arial, Helvetica, sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    list-style: none;
    text-decoration: none;
  }

  .main-container {
    margin: 50px;
    min-height: 250px;
  }

  h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }
</style>
