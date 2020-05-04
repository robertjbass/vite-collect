<template>
  <Main />
</template>

<script>
import Main from "./components/Main.vue";
export default {
  name: "App",
  data: () => ({ foo: "bar" }),
  setup() {
    console.log("Vite App is running");
  },
  components: {
    Main
  }
};
</script>

<style scoped>
/* 
Vue Blue: #34495E (Police Blue)
Vue Green: #41B883 (Mint)
*/
* {
  font-family: "Courier New", Courier, monospace;
}
</style>
