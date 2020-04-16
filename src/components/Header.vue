<template>
  <div class="header-main">
    
    <img width="140px" src="/src/assets/pagina3.png" >

    <div class="header-buttons">
      <img class="iconsearch" src="/icons/search.png" alt="search" >
     
      <input type="search" class="busqueda" placeholder="Buscar productos,marcas y mas...">
     <!--  <p class="button-support">Buscar</p> -->
         
      <!-- <div class="button-support-border">
        <p>Iniciar sesión</p>
      </div> -->
    </div>
    
  </div>
  
  
</template>

<script>
export default {};
</script>

<style scoped>

.busqueda{

display: flex;
align-items: center;
justify-content: space-between;
width: 526px;
height: 32px;
left: 457px;
top: 14px;

background: #F4ECEC;
border-radius: 10px;

}
.iconsearch{
display: flex;
align-items: center;
justify-content: space-between;

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
  width: 850px;
  height: 45px;
  align-items: center;
  justify-content: space-between;
}
.button-support {
  color: #1a059b;
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
}
.button-support-border {
  display: flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(
    270deg,
    #5b7cf0 0%,
    rgba(88, 31, 249, 0.94) 67.59%
  );
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  border-radius: 7px;
  padding: 3px;
  height: 35px;
  width: 150px;
}
.button-support-border p {
  color: white;
  padding: 0px;
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
}
</style>
