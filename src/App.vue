<template>
  <TheHeader v-show="showHeader" />
  <TheList/>
</template>

<script>
import TheHeader from "./components/TheHeader";
import TheList from "./components/TheList"

export default {
  name: "App",
  components: {
    TheHeader,
    TheList,
  },
  data() {
    return {
      showHeader: true // Verifique se isso está definido como true
    };
  },
};
</script>


<style>
body {
  background: #232323;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 60px;
  background: #232323;
}
</style>
