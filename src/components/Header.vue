<template>
  <div class="header-main">
    <img width="60px" src="../assets/pagina3.png" />

    <!-- agregar imagenes de assets se hace con la forma de abajo -->

    <!-- <button @click="ejemplo">esconder</button>
    <button @click="reaparecer">aparecer</button> -->
      
    <div class="header-buttons">
      
      <ul class="submenu">
        <li >
          <transition name="fade">
            <ul v-if="Categoria" @click="Categoria = false">
              <li><a href="#">Sub menu</a></li>
              <li><a href="#">Sub menu</a></li>
              <li><a href="#">Sub menu</a></li>
            </ul>
          </transition>
        </li>
      </ul>
      <img  @mouseover="Categoria = true" @mouseleave="Categoria = false" 
      class="imagen" src="../assets/categoria.png" alt=""/>
      <div class="menu">
        <input
          type="search"
          class="busqueda"
          placeholder="Buscar productos,marcas y mas..."
        />
        <img src="../assets/search.png" alt="search" />
        <img src="../assets/account.png" alt="account" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      menu: true,
      Categoria: false,
    };
  },
  methods: {
    reaparecer() {
      this.muestraLogo = true;
    },
    ejemplo() {
      this.muestraLogo = true;
    },
  },
};
</script>

<style scoped>
.submenu {
  display: flex;
}
.imagen{
  display: flex;
  
}
.submenu li {
  list-style: none;
}
.submenu li a {
  display: flex;
  justify-content: flex-end;
  flex: end;
  background: chartreuse;
  
}
.menu li ul li {
  background: #fff;
  transition: background 0.2s;
}
.menu li ul li:hover {
  background: #444;
}
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.2s;
}
.fade-enter,
.fade-leave-active {
  opacity: 0;
}
.menu {
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
