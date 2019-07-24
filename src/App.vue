<template>
  <div id="app">
    <Home></Home>
  </div>
</template>
<script>
  import Home from '@/components/Home'
  export default {
    name: 'App',
    components: {
      'Home': Home
    }
  }
</script>
<style>
  #app {
    text-align: center;
    margin-top:400px ;
  }
</style>
