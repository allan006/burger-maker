<script>
import Navbar from "./components/Navbar.vue"
import Footer from "./components/Footer.vue"

export default{
  components: { 
    Navbar,
    Footer,
  },
  data() {
    return {
      logo_src: "img/logo.png",
      app_name: "Burger Maker"
    }
  }
}
</script>

<template>
  <Navbar :logo="logo_src" :alt="app_name" />
  <RouterView />
  <Footer />
</template>

<style>
  *{
    font-family: Helvetica;
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
  }

  .main-container{
    margin: 50px;
    min-height: 250px;
  }

  h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }

  #main-banner h1 {
    color: #FFF;
    text-align: center;
    font-size: 60px;
    padding: 20px 40px;
  }
</style>
