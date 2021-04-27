<template>
  <div id="app">
    <Header/>
    <AllTask/>
    <AllTaskForm/>

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

</style>
