<template>
  <div id="app">
    <!--左侧导航-->
    <leftNav></leftNav>
    <!--操作区域-->
    <router-view></router-view>
  </div>
</template>

<script>
import leftNav from './components/common/leftNav.vue'
export default {
  name: 'app',
  components:{
      leftNav
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  height: 100%;
}
.main{
  float:left;
  width:95%;
  background-color: #EFF2F7;
  height:100%;
  overflow: auto;
}
</style>
