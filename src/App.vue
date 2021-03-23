<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
import mainBody from './components/mainBody'
export default {
  name: 'App',
  components: { mainBody }
}
</script>

<style>
#app{
  width: 100%;
  height: 100vh;
}
body{
  padding: 0;
  margin: 0;
}
</style>
