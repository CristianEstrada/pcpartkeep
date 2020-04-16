<template>
  <div class="header-main">
    
    <img width="140px" src="" />

    <div class="header-buttons">
      <!-- agregar imagenes de assets se hace con la forma de abajo -->

    <button @click="ejemplo">esconder</button>
    <button @click="reaparecer">aparecer</button>
      <img src="../assets/categoria.png" alt="">
      <input type="search" class="busqueda" placeholder="Buscar productos,marcas y mas...">
      <img  v-if="muestraLogo" src="../assets/search.png" alt="search" />
      <img src="../assets/account.png" alt="account" />
      

      
     
    </div>
    
  </div>
  
  
</template>

<script>
export default {
 
  data() {
    return {
      muestraLogo: true,
    }
  },
   methods:{
    reaparecer(){
      this.muestraLogo = true;
    },
    ejemplo(){
      this.muestraLogo = false;
    }
  },
}
</script>

<style scoped>

.busqueda{

display: flex;

width: 526px;
height: 32px;
left: 457px;
top: 14px;

background: #F4ECEC;
border-radius: 10px;

}
.iconsearch{
display: flex;
align-items: flex-end;

}
.header-main {
 /* Header */

display: flex;
align-items: center;
height: 60px;

/* White Base */

background: #FFFFFF;
 position: absolute;
left: -1px;
right: -1px;
top: -1px;
bottom: -1px;
border: 1px solid #4D94FF;
display: flex;
}
.header-buttons {
  display: flex;
  width: 1440px;
  height: 45px;
  align-items: center;
  justify-content: space-between;
}


.button-support-border p {
  color: white;
  padding: 0px;
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
}
</style>
