<template>
  <h3>Notations</h3>
  <!--form-->
  <input id="note" v-model="note" placeholder="edit me"><br>{{note}}</input>
  <br />
  <button v-on:click="note='addToArray'"> Save</button><br>{{note}}<br>
  <button v-on:click="note=addNotation()">Save</button>
  
 
  <div v-for="notation in notations">{{ notation }}<br /></div>
  <!--/form-->
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
    addNotation() {
       note = "methodWorked"
         return note
      }
    }
}
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
  font-size: 20px;
  font-weight: bold;
}
</style>
