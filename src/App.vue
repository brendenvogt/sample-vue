<template>
  <Header/>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/name">Name</router-link> |
    <router-link to="/counter">Counter</router-link>
  </div>
  <router-view/>
  <Footer user="Hello"/>
</template>

<script>
import Footer from './components/Footer.vue';
import Header from './components/Header.vue';

export default {
  components: {
    Footer,
    Header,
  },
};
</script>

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
