<template>
  <div class="todo-body">
    <div class="tasks">
        <Task taskId="task-1" taskMessage="Teste Texto 1"/>
        <Task taskId="task-2" taskMessage="Teste Texto 2"/>
        <Task taskId="task-3" taskMessage="Teste Texto 3"/>
    </div>

    <div class="new-task-creator">
        <CreateTaskForm makeTask="task"/>
    </div>

    <div class="delete-buttons">
      <DeleteListButton buttonText="Limpar Completados"/>
      <DeleteListButton buttonText="Deletar Lista"/>
    </div>
  </div>
</template>

<script>

import Task from './TodoListTasks'
import CreateTaskForm from '../../Forms/AllTaskForm'
import DeleteListButton from '../../Buttons/DeleteButton'

export default {
    components:{
        Task,
        CreateTaskForm,
        DeleteListButton
    }
};
</script>

<style>

.todo-body{
  padding: 2rem;
}

[type="checkbox"]{
  opacity: 0;
  position: absolute;
}

</style>
