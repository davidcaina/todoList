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

<style scoped>

</style>
