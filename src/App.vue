<template>
  <div id="app">
    <!--<img src="./assets/logo.png">-->
    <!--<h1>Frameworks Filter</h1>-->
    <hello></hello>
  </div>
</template>

<script>
  import Hello from './components/Hello'

  export default {
    name: 'app',
    components: {
      Hello,
    }
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }
  /*h1*/
  /*{*/
    /*text-align: center;*/
    /*font-family: "Adobe Caslon Pro";*/
    /*color: #b6c7ff;*/
  /*}*/

</style>
