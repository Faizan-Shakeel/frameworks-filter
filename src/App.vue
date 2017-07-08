<template>
  <div id="app">
    <!--<img src="./assets/logo.png">-->
    <!--<h1>Frameworks Filter</h1>-->

    <hello></hello>

  </div>
</template>

<script>
  import Hello from './components/Framework-Filter'

  export default {
    name: 'app',
    components: {
      Hello,
    }
  }
</script>

<style>
  #app {
    font-family: 'Quicksand', sans-serif;
    letter-spacing: 1px;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

</style>
