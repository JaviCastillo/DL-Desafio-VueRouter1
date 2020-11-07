<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark px-5">
      <a class="navbar-brand" href="#">V8</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
        <font-awesome-icon :icon="['fas','bars']" />
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <!-- MENU DE NAVEGACION -->
        <div class="navbar-nav ml-auto">
          <!-- REEMPLAZAR CON ELEMENTO ROUTER LINK A CON RUTA NOMBRADA -->
          <router-link class="nav-link" :to="{name: 'Portada'}">Portada</router-link>
          <!-- REEMPLAZAR CON ELEMENTO ROUTER LINK A CON RUTA NOMBRADA -->
          <router-link class="nav-link" :to="{name: 'SobreMi'}">Sobre Mi</router-link>
          <!-- REEMPLAZAR CON ELEMENTO ROUTER LINK A RUTA ESTÁTICA -->
          <router-link class="nav-link" to="/contacto">Contacto</router-link>
          <!-- REEMPLAZAR CON ELEMENTO ROUTER LINK A RUTA ESTÁTICA -->
          <router-link class="nav-link" to="/post/1">Blog</router-link>
        </div>
      </div>
    </nav>

    <!-- ROUTER VIEW QUE CARGARÁ LAS VISTAS (INICIO, SOBRE MÍ, CONTACTO, ETC.) -->
    <router-view></router-view>
  </div>
  
</template>

<style scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;  
}

#menu-v8 a{
  text-shadow: 1px 1px #000;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
