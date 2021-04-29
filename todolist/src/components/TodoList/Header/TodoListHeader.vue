<template>
    <div class="todolist-header2">
        <h2 class="todolist-header"> Titulo Todo </h2>
        <TodoListHeaderCounter/>
    </div>
</template>

<script>

import TodoListHeaderCounter from './TodoListHeaderCounter'

export default {
    components:{
        TodoListHeaderCounter
    }
};
</script>

<style>

.todolist-header2{
    background: #e4e4e4;
    margin: 0;
    padding: 2rem;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.todolist-header{
    margin: 0 1em 0 0;
}

</style>
