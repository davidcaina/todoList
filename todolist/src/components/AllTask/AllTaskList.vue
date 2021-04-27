<template>
    <ul class="all-task-list">
        <Elemento nomeElemento="Test1"/>
        <Elemento nomeElemento="Test2"/>
        <Elemento nomeElemento="Test3"/>
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

<style scoped>

</style>
