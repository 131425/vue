<template>
  <!--顶部bar-->
  <mu-appbar class="HeaderBar">
    <p class="p">Vue.js项目</p>
  </mu-appbar>
</template>

<style scoped>
  .HeaderBar {
    position: fixed;
    top: 0;
    height: 4rem;
  }
  
  .appbar-search-field {
    color: #FFF;
    margin-bottom: 0;
  }
  
  .appbar-search-field.focus-state {
    color: #FFF;
  }
  
  .appbar-search-field .mu-text-field-hint {
    color: rgba(255, 255, 255, 0.54);
  }
  
  .appbar-search-field .mu-text-field-input {
    color: #FFF;
  }
  
  .logo {
    width: 4rem;
    height: 4rem;
    position: absolute;
    left: 0;
    top: 0;
  }
</style>