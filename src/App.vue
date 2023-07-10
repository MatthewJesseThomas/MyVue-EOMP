<template>
  <NavBar/>
  <main>
    <router-view/>
  </main>
  <Footer/>

</template>
<script>
import NavBar from './components/NavBar.vue'
import Footer from './components/Footer.vue'
export default {
  components: {
    Footer,
    NavBar
  }
};
</script>
<style>
#app {
  font-family: 'Oswald', sans-serif;
  font-family: 'Share Tech', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  overflow-x: hidden;
  overflow-y: hidden;
  background-image: linear-gradient(to right, #101b37 30%, #e41376);
  background-size: cover;
  background-repeat: no-repeat;
  min-height: 100vh;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #d3e7f9;
  text-decoration: none !important;

}

nav a.router-link-exact-active {
  color: #F0F8FF;
  text-decoration: none !important;
  
}
main{
  z-index: 2;
}
/* 
background: #e8cbc0;
background: -webkit-linear-gradient(to right, #e8cbc0, #636fa4);
background: linear-gradient(to right, #e8cbc0, #636fa4);
*/
</style>
