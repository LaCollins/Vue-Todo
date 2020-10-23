<template>
  <div id="app">
    <div id="nav">
      <Header />
    </div>
    <router-view/>
  </div>
</template>

<script>
import Header from './components/layout/Header';

export default {
  name: "app",
  components: {
    Header
    }
    }
</script>

<style>
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    }

  body {
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.4;
    margin: 20px;
    padding: 20px;
    }

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 0px;
}

#nav a {
  font-weight: bold;
  color: #487097;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
