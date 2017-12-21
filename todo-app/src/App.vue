<template>
  <div id="app">
    <img src="./assets/logo.png">
    <HelloWorld/>
    <ToDoList/>
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
