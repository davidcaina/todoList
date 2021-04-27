<template>
  <div id="all-task-id" class="all-tasks">
      <h2>Minha Lista</h2>
      <AllTaskList/>
  </div>
</template>

<script>

import AllTaskList from "./AllTaskList"

export default {
  components: {
    AllTaskList,
  },
};
</script>

<style scoped>

</style>
