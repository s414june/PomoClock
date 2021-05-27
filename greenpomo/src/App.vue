<template>
  <div id="app">
    <header-com></header-com>
    <pomo-com></pomo-com>
  </div>
</template>

<script>

import HeaderCom from './components/header-com.vue'
import PomoCom from './components/pomo-com.vue'

export default {
  name: 'App',
  components: {
    HeaderCom,
    PomoCom
  },
  data(){
 
  return{
  
    }
  }
}
</script>

<style>
  :root {
        font-family: 'Noto Sans TC', sans-serif;
        --green: #399;
        --main-font-size: calc(1.5rem + 1vw);
        overflow-x: hidden;
    }
    
    body {
        margin: 0;
    }
</style>
