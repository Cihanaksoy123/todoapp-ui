<template>
  <div id="app">
    <div v-if="isLoggedIn">
      <NavBar />
      <router-view />
    </div>
    <div v-if="!isLoggedIn"><LoginView /></div>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from "./components/NavBar.vue";
import LoginView from "./views/Login.vue";
export default {
  name: "App",
  components: { NavBar, LoginView },
  data: function () {
    return {
      isLoggedIn: false,
    };
  },
};
</script>



<style lang="scss">
body {
  display: flex; //added
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  align-self: center; //added
  flex: auto; //added
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
