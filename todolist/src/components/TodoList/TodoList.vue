<template>
    <div class="todo-list">
    <TodoListHeader/>
    <TodoListBody/>
    </div>
</template>

<script>

import TodoListHeader from './Header/TodoListHeader'
import TodoListBody from './Body/TodoListBody'

export default {
    components: {
        TodoListHeader,
        TodoListBody
    }
};
</script>

<style>
.todo-list{

  position: absolute;
  transform: translate(850px, 150px);

  background: var(--light-color);
  color: var(--dark-color);
}
</style>
