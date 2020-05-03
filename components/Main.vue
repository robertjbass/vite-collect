<template>
  <div>
    <h1>This is my Vite Main Component</h1>
    <h3>Vite + Vue 3!</h3>
    <p>
      <span>Count is: {{ count }}</span
      ><br />
      <button @click="count++">increment</button><br />
      <button @click="count--">decrement</button>
    </p>
  </div>
</template>

<script>
export default {
  name: "Main",
  data: () => ({ count: 0 })
  // setup() {
  //   console.log("Main.vue component is running");
  // }
};
</script>

<style scoped>
* {
  font-family: "Courier New", Courier, monospace;
}

h1 {
  color: #4fc08d;
}

p {
  margin: auto;
}

button {
  background-color: #4fc08d;
}
</style>
