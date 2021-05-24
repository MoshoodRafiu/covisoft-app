<template>
  <div id="app">
    <app-navbar/>
    <router-view/>
  </div>
</template>

<script>
  import appNavbar from '@/components/Navbar';
  export default {
    data(){
      return{
      }
    },
    components: {
      appNavbar
    }
  }
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@100;300;400;500;700;900&display=swap');
  :root {
    --purple: #7D00A9;
    --purple-hover: #540072;
    --black: #000000;
    --white: #ffffff;
  }
  #app{
    font-family: 'Noto Sans JP', sans-serif;
    width: 100%;
    overflow-x: hidden;
  }
</style>
