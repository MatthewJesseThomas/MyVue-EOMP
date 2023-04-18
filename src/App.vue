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
  font-family: 'Avenir', 'Helvetica', 'Arial', 'sans-serif';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  overflow-x: hidden;
  overflow-y: hidden;
  background-image: url(https://i.postimg.cc/63s4CfdH/efe-kurnaz-Rn-CPi-Xixoo-Y-unsplash.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  min-height: 100vh;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
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
