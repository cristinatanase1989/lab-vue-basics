<template>
<nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a class="navbar-item" href="https://bulma.io">
      <img src="https://www.norwegian.com/Content/img/ident.svg" width="300">
    </a>

    <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>

  <div id="navbarBasicExample" class="navbar-menu">
    <div class="navbar-start">
      <a class="navbar-item">
        Home
      </a>

      <a class="navbar-item">
        Documentacion para viajar
      </a>

      <div class="navbar-item has-dropdown is-hoverable">
        <a class="navbar-link">
         Viajes
        </a>

        <div class="navbar-dropdown">
          <a class="navbar-item">
            Europa
          </a>
          <a class="navbar-item">
            America
          </a>
          <a class="navbar-item">
           Asia
          </a>
          <hr class="navbar-divider">
        
        </div>
      </div>
    </div>

    <div class="navbar-end">
      <div class="navbar-item">
        <div class="buttons">
          <a class="button is-info">
            <strong>Iniciar sesion</strong>
          </a>
          <a class="button is-success button is-large">
           Buscar vuelos
          </a>
        </div>
      </div>
    </div>
  </div>
</nav>

</template>
<script setup>
</script>
<style scoped>
.navbar{
    background-color: red;
}

.navbar-menu{
text-shadow: 1px 1px 9px rgb(50, 6, 154);

}
</style>