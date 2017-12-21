<template>
  <div id="app">
    <img src="./assets/logo.png">
    <HelloWorld/>
    <ToDoList v-bind:todos="todos"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import ToDoList from './components/ToDoList'

export default {
  name: 'app',
  components: {
    HelloWorld,
    ToDoList
  },
  data() {
    return {
      todos: [{
        title: 'Todo A',
        project: 'Project A',
        done: false,
      }, {
        title: 'Todo B',
        project: 'Project B',
        done: true,
      }, {
        title: 'Todo C',
        project: 'Project C',
        done: false,
      }, {
        title: 'Todo D',
        project: 'Project D',
        done: false,
      }],
    };
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
