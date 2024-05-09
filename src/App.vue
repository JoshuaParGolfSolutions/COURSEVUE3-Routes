<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>|
    <router-link to="/services">Services</router-link>|
    <router-link to="/blog">Blog</router-link>|
    <router-link to="/contacts">Contacts</router-link>|
  </nav>
  <router-view />
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  li {
    padding: 30px;
    position: relative;
    font-weight: bold;
    color: #2c3e50;
    list-style: none;
  }
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    //Este es el que hace que se ponga en color segun la ruta activa. Ver en 'inspeccionar'
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
