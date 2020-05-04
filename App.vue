<template>
  <Main />
  <BodyForm />
</template>

<script>
import Main from "./components/Main.vue";
import BodyForm from "./components/BodyForm.vue";

export default {
  name: "App",
  setup() {
    console.log("Vite App is running");
  },
  components: {
    Main,
    BodyForm
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
