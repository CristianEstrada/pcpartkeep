<template>
  <div class="header-main">
    
      <img width="60px" src="../assets/pagina3.png" />

 <!-- agregar imagenes de assets se hace con la forma de abajo -->

        <!-- <button @click="ejemplo">esconder</button>
    <button @click="reaparecer">aparecer</button> -->

      <div class="header-buttons">
          <div class="menu">
        <img src="../assets/categoria.png" alt="" />
        <input
          type="search"
          class="busqueda"
          placeholder="Buscar productos,marcas y mas..."/>
        
          <img v-if="muestraLogo" src="../assets/search.png" alt="search" />
          <img src="../assets/account.png" alt="account" />
        </div>
      </div>
    </div>
  
</template>

<script>
export default {
  data() {
    return {
      muestraLogo: true,
    };
  },
  methods: {
    reaparecer() {
      this.muestraLogo = true;
    },
    ejemplo() {
      this.muestraLogo = false;
    },
  },
};
</script>

<style scoped>
.menu{
  display: flex;
}
.busqueda {
  display: flex;

  width: 526px;
  height: 32px;
  left: 457px;
  top: 14px;

  background: #f4ecec;
  border-radius: 10px;
}
.iconsearch {
  display: flex;
  align-items: flex-end;
}
.header-main {
  /* Header */

  display: flex;
  align-items: center;
  justify-content: center;
 

  height: 60px;

  /* White Base */

  background: #ffffff;
  position: absolute;
  left: -1px;
  right: -1px;
  top: -1px;
  bottom: -1px;
  border: 1px solid #4d94ff;
  display: flex;
}
.header-buttons {
  display: flex;

  
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
