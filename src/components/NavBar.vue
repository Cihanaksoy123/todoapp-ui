<template>
  <div id="app">
    <div id="nav">
      <router-link to="/login">Login</router-link> |
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
  </div>
</template>
<script>
export default {
  name: "NavBar",
  data: function () {
    return {
      data: 0,
    };
  },
};
</script>