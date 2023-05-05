<template>
  <div>
    <h2>Todo List</h2>
      <form v-on:submit.prevent>
        <input type="text" v-model="newItem">
        <button v-on:click="addItem">Add</button>
      </form>
      <pre>{{ $data }}</pre>
  </div>
</template>

<script>
export default {
  name: 'Todo',
  data() {
    return {
      newItem: ''
    }
  },
  methods: {
    // eslint-disable-next-line no-unused-vars
    addItem: function(event) {
      console.log('Clicked!')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
