<template>
  <h3>Notations</h3>
  <input v-model="note" placeholder="-" />
  <p>updateArray()</p>
  <button v-on:click="updateArray()">Save</button>
  <br />
  <br />
  <p>addNotation()</p>
  <button v-on:click="note = addNotation()">
    Save
  </button>
  <div>
    <div v-for="notation in notations">
      {{ notation }}
    </div>
    <br /><br />
    Variables:
    <br /><br />
    Notations: {{ notations }}
    <br />
    Note: {{ note }}
  </div>
  <br />
</template>

<script>
export default {
  name: "BodyForm",
  data() {
    return {
      notations: ["A", "B", "C"]
    };
  },
  methods: {
    addNotation(note) {
      let addToArray = note;
      note = notations;
      return note;
    },
    updateArray(notations) {
      console.log(notations);
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
