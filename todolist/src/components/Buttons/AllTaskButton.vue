<template>
    <button v-if="makeTask == 'list'" class="btn list" aria-label="criar nova lista">+</button>
    <button v-else-if="makeTask == 'task'" class="btn task" aria-label="criar nova task">+</button>
</template>

<script>

export default {
    props: {
        makeTask: {type: String, required: true}
    }
};
</script>

<style scoped>

</style>
