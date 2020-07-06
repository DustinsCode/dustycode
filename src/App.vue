<template>
  <v-app>
    <v-content>
      <v-toolbar app>
        <v-toolbar-title class="headline text-uppercase">
          <span>Dustin R Thurston</span>
          
          <router-link to="/">Home</router-link>
          <router-link to="/about">About</router-link>
        </v-toolbar-title>
      </v-toolbar>
      <router-view></router-view>
    </v-content>
  </v-app>
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
      color: #42b983;
    }
  }
}
</style>
