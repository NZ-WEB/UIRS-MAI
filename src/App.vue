<template>
  <div id="app">
    <div id="nav">
      <router-link to="/system">System</router-link>
      | <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
    <v-footer class="mt-5" >
      <v-col
          class="text-center"
          cols="12"
      >
        {{ new Date().getFullYear() }} — <span>M30-204C-19</span>
      </v-col>
    </v-footer>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #3F51B5;
    }
  }
}
</style>
