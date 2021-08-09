<template>

    <b-navbar toggleable="md">
      <b-navbar-toggle target="navbar-toggle-collapse">
        <template #default="{ expanded }">
          <b-icon v-if="expanded" icon="chevron-bar-up"></b-icon>
          <b-icon v-else icon="chevron-bar-down"></b-icon>
        </template>
      </b-navbar-toggle>

      <b-collapse id="navbar-toggle-collapse" is-nav>
        <nav>
          <ul class="topnav sticky-navbar">
            <li class="right">
              <NuxtLink to="/">Inicio</NuxtLink>
            </li>
                      <li class="right">
                        <NuxtLink to="/servicios">Servicios</NuxtLink>
                      </li>
                      <li class="right">
                        <NuxtLink to="/about">Nosotros</NuxtLink>
                      </li>
                      <li class="right">
                        <NuxtLink to="/contact">Contacto</NuxtLink>
                      </li>
                      <li class="right">
                        <NuxtLink to=" /login">Inicia sesión</NuxtLink>
                      </li>
          </ul>
        </nav>
      </b-collapse>
    </b-navbar>
</template>
<script>
export default {

}
</script>
<style>
@import url(https://fonts.googleapis.com/css?family=Lobster);

ul.topnav {
  list-style-type: none;
  padding-top: 40px;
  overflow: hidden;
  background-color: white;
}

ul.topnav li {
  float: right;
}

ul.topnav li a {
  display: block;
  color: black;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

ul.topnav li a:hover:not(.active) {
  background-color: #d5e2d6;
  color: black;
  border-radius: 5px;
}

ul.topnav li a.active {
  background-color: #d5e2d6;
  color: black;
}

ul.topnav li.right {
  float: left;
}

@media screen and (max-width: 600px) {
  ul.topnav li.right,
  ul.topnav li {
    float: none;
  }
}
</style>
