<template>
  <div id="app">
    <Todos v-bind:todos = "todos"></Todos>
  </div>
</template>

<script>

import Todos from './components/Todos';

export default {
  name: 'app',
  components: {
    Todos
  },

  data()
  {
    return{
      todos: 
      [
        {
          id: 1,
          title: "To do one",
          completed: false
        },
        {
          id: 2,
          title: "To do two",
          completed: true
        },
        {
          id: 3,
          title: "To do three",
          completed: false
        }
      ]
    }
  }
}
</script>

<style>
*
{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body
{
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
</style>
