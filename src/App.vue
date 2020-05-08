<template>
  <div>
    <div class="main">
      
      <Header />  
     
      <Body /> 
      
      <Footer />
      
    </div>
  </div>
</template>

<script>
import Header from "./components/Header";

import Footer from "./components/Footer";
import Body from "./components/Body";


export default {
  name: "App",
  components: { Header,
  Footer, 
  Body,
  }
};
</script>

<style scoped>
.main {

 
}
</style>