<template>
<narbar/>
<router-view></router-view>
</template>

<script>
  import Narbar from "./components/NavBar.vue";

  export default {
    name:"App",
    components:{
      Narbar,
    }
};

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
