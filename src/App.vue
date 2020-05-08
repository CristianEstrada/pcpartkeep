<template>
  <div>
    <div class="main">
      
      <Header />  
     
      <Body /> 
       <Menu />
      <Footer />
      
    </div>
  </div>
</template>

<script>
import Header from "./components/Header";
import Menu from "./components/Menu";
import Footer from "./components/Footer";
import Body from "./components/Body";


export default {
  name: "App",
  components: { Header,
  Footer, 
  Body,
  Menu }
};
</script>

<style scoped>
.main {
  display: flex;
  flex-direction: column;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  width: 100%;
  height: 100vh;
}
</style>