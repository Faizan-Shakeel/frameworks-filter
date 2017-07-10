<template>
  <div id="app">

    <Framework-Filter></Framework-Filter>

  </div>
</template>

<script>
  import FrameworkFilter from './components/Framework-Filter'

  export default {
    name: 'app',
    components: {
      FrameworkFilter
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
