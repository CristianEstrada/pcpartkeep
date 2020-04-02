<template>
  <div class="header-main">
    <img width="140px" src="" />

    <div class="header-buttons">
      <p class="button-support">Inicio</p>
      <p class="button-support">Soporte</p>
      <input type="search" class="busqueda" placeholder="Buscar productos,marcas y mas...">
      <p class="button-support">Buscar</p>
         
      <div class="button-support-border">
        <p>Iniciar sesión</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.busqueda{
  
  padding: 0px;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
   box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  border-radius: 7px;
  padding: 3px;
  height: 25px;
  width: 350px;
}
.header-main {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 90%;
  height: 55px;
  background: #ffffff;
  box-shadow: 0px 2px 0px rgba(0, 0, 0, 0.25);
  padding: 0px 50px;
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
