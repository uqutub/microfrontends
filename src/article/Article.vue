<template>
  <div id="article">
    <div>
      <b>Article >> </b>
      <router-link to="/">Article Home</router-link> |
      <router-link to="/add">Add Article</router-link>
    </div>
    <router-view />
  </div>
</template>

<script>
import { mapActions, mapMutations, mapState } from 'vuex';
import { navigateTo } from '../shared/helper/index';
export default {
  components: {},
  methods: {
    navigateTo
  }
};
</script>

<style lang="scss">
:root {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
}
#article {
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>

