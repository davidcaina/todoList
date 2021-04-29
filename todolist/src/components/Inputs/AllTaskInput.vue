<template>

    <input v-if="makeTask == 'list'" type="text"  class="new list" :placeholder="placeHolderList" :aria-label="placeHolderList">
    <input v-else-if="makeTask == 'task'" type="text"  class="new task" :placeholder="placeHolderTask" :aria-label="placeHolderTask">
</template>

<script>

export default {
    data(){
        return {
            placeHolderList: "nome da nova lista",
            placeHolderTask: "nome da nova task"
        }
    },
    props: {
        makeTask: {type: String, required: true}
    }
};
</script>

<style scoped>

</style>
