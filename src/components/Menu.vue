<template>
    <div id="app">
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
        
</div>
</template>

<script>
export default {
    data(){
        return{
        Categoria: false,
        }
    },
}
</script>

<style  scoped>
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
</style>