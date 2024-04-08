<template>
  <div id="app">
    <Header />
    <router-view/>  
    <Footer />
  </div>
</template>

<script>
import Footer from './components/Footer.vue';
import Header from './components/Header.vue';





export default {
  components:{
    Header,
    Footer

  },

}
</script>

<style>
*{
  list-style: none;
  margin: 0;
  padding: 0;
  font-family: Helvetica;
  text-decoration: none;
  color: black;
}
</style>
