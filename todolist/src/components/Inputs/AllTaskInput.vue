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

<style>

.new {
    background: transparent;
    border: 0;
    color: #f4f4f4;
    border-bottom: 1px solid currentColor;
    font-size: inherit;
    outline: none;
    transition: border-bottom 150ms ease-in;
    order: 2;
}

.new:focus{
    border-bottom-width: 3px;
}

.new:focus::placeholder{
    opacity: 0.2;
}

.new.list{
    font-size: 1rem;
}
</style>
