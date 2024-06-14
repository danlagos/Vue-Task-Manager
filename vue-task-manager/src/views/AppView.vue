<template>
    <div class="app-layout">
      <HeaderComp />

    </div>
  </template>
  
  <script>
import HeaderComp from '../components/HeaderComp.vue'
  
  export default {
    name: 'AppLayout',
    components: {
      HeaderComp 
    }
  }
  </script>
  
  <style scoped>
  .app-layout {
    display: flex;
    flex-direction: column;
    align-items: stretch;
    min-height: 100vh;
  }
  </style>
  