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
* {
  font-family: "Courier New", Courier, monospace;
}
</style>
