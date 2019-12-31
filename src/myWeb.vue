<template>
  <div id="myWeb">
    <div class="loading" v-show="loading">
      <div class="icon"><img src="../static/timg.gif" /></div>
    </div>
    <router-view />
  </div>
</template>

<script>
export default {
  name: 'myWeb',
  data(){
    return{
      loading:true
    }
  }
};
</script>

<style>
#myWeb {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: black;
}
.loading {
  position: fixed;
  width: 100%;
  height: 100%;
  z-index: 100;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
