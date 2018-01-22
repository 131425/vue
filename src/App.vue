<template>
  <div id="app">
    <router-view></router-view>   
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
html{
  font-size: 62.5%;
 
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
::-webkit-scrollbar {
    width: 2px;
    height: 2px;
}

::-webkit-scrollbar-track {
    background: transparent;
}

::-webkit-scrollbar-thumb {
    background: rgba(0,0,0,.1);
}
</style>
