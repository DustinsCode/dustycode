<template>
  <v-app dark>
      <app-navigation></app-navigation>
      <v-main>
        <v-container fluid style="padding: 0; height: 100%; width: 100%;">
          <router-view></router-view>
        </v-container>
      </v-main>
      <v-footer>
        Footer things
      </v-footer>
  </v-app>
</template>

<script>
import AppNavigation from '@/components/AppNavigation'

export default {
  name: 'App',
  components: {
    AppNavigation
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // color: #2c3e50;
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
