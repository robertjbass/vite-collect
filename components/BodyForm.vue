<template>
  <h3>Notations</h3>
  <input id="note" v-model="note" placeholder="edit me" />
  <br />{{ note }}<br />
  <p>Input Text</p>
  <button v-on:click="note = 'addToArray'">Save</button>
  <br /><br />
  <p>Run Method</p>
  <button v-on:click="note = addNotation()">Save</button>
  <div v-for="notation in notations">
    {{ notation }}
  </div>
  <br />
</template>

<script>
export default {
  name: "BodyForm",
  data() {
    return {
      note: "blankNote",
      notations: ["1", "2", "3", "4", "5"]
    };
  },
  methods: {
    addNotation(note) {
      let addToArray = note;
      return (note = "Method Ran");
      return addToArray;
    }
  }
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
  color: #4fc08d;
  background-color: #34495e;
  font-size: 20px;
  font-weight: bold;
}
</style>
