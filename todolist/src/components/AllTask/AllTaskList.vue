<template>
    <ul class="all-task-list">
        <Elemento nomeElemento="Test1" isActive="active"/>
        <Elemento nomeElemento="Test2" isActive=""/>
        <Elemento nomeElemento="Test3" isActive=""/>
    </ul>
</template>

<script>

import Elemento from "./AllTaskListElements"

export default {
  components: {
    Elemento,
  },
};
</script>

<style>

.all-task-list{
  font-size: 1.2rem;
  padding-left: 1em;
  line-height: 1.7;
  list-style: circle;
}
</style>
