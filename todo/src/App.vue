<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <Todo v-bind:todos='todos'></Todo>
  </div>
</template>

<script>
import Todo from './components/Todo'

export default {
  name: 'App', // hello 
  components: {
    Todo,
  },
  // data function adds data to the template.
  data() {
    return {
      todos: [{
        title: 'Todo A',
        project: 'Project A',
        done: false,
      }, {
        title: 'Todo B',
        project: 'Project B',
        done: false,
      }, {
        title: 'Todo C',
        project: 'Project C',
        done: true,
      }, {
        title: 'Todo D',
        project: 'Project D',
        done: false,
      }],
    };
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /* margin-top: 60px; */
}
</style>
