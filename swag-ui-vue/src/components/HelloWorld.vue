<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      For a guide and recipes on how to design SoftWare Architecture <br>
      check out the
      <a href="https://github.com/jhnjslee/swarchguide" target="_blank" rel="noopener">Github</a>.
    </p>
    <h3>API Test</h3>
    <ul>
      <button @click="createItem()">Create</button>
      <button @click="createItem()">Read</button>
      <button @click="createItem()">Update</button>
      <button @click="createItem()">Delete</button>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
//  data() {},
  methods: {
    createItem() {
      console.log("create Item")
    }
  },
}



</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #3337b5;
}
</style>
