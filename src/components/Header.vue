<template>
  <div>
  <b-navbar toggleable="lg" type="light" style="background-color: #fffff">
    <b-navbar-brand href="#">
      <img src="../assets/pagina3.png" style="width: 60px" alt="">
    </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#">Link</b-nav-item>
        <b-nav-item href="#" disabled>Disabled</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Buscar"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="search">Buscar</b-button>
        </b-nav-form>

        <b-nav-item-dropdown text="Lenguaje" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
          <b-dropdown-item href="#">RU</b-dropdown-item>
          <b-dropdown-item href="#">FA</b-dropdown-item>
        </b-nav-item-dropdown>

        <b-nav-item-dropdown right>
          <!-- Using 'button-content' slot -->
          <template v-slot:button-content>
            <em>Usuario</em>
          </template>
          <b-dropdown-item href="#">Perfil</b-dropdown-item>
          <b-dropdown-item href="#">Cerrar Sesion</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
  <div class="linea">

  </div>
</div>
</template>

<script>
export default {
  data() {
    return {
      menu: true,
      Categoria: false
    };
  },
  methods: {
    reaparecer() {
      this.muestraLogo = true;
    },
    ejemplo() {
      this.muestraLogo = true;
    }
  }
};
</script>

<style scoped>
.linea {
  /* Header */
  

  /* White Base */

  
  left: -1px;
  right: -1px;
  top: -1px;
  bottom: -1px;
  border: 1px solid #4d94ff;
  
}
</style>
