<template>
  <div id="app">
    <Header/>
    <div class="all-tasks1">
      <AllTask/>
      <AllTaskForm makeTask="list"/>
    </div>
    <TodoList/>
  </div>
</template>

<script>

// Todo List -> Esquerda
import Header from './components/Header/Header'
import AllTask from './components/AllTask/AllTask'
import AllTaskForm from './components/Forms/AllTaskForm'


// Todo List -> Direita
import TodoList from './components/TodoList/TodoList'

export default {
  name: 'App',
  components:{
    Header,
    AllTask,
    AllTaskForm,
    TodoList
  }
}
</script>

<style>
:root{
  --primary-color: rgb(54, 112, 199);
  --warning-color: rgb(99, 36, 36);
  --dark-color: #333;
  --light-color: #f4f4f4;

}

*,
*::before,
*::after {
  font-family: inherit;
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: "Work Sans", sans-serif;
  font-weight: 300;
  font-size: 1.5rem;
  background: var(--primary-color);
  color: var(--light-color);

}

</style>
