<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
  *{
    margin:0;
    padding:0;
    user-select:none;
  }
  li{
    list-style:none;
  }
  a{
    text-decoration: none;
    outline:none;
  }
  html,body{
    width:100vw;
    height:100%;
    font:1em "poppin","Microsoft YaHei", "SimSun", "SimHei", Arial;
  }
  
</style>
