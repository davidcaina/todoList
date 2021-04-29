<template>
    <button v-if="makeTask == 'list'" class="btn create" aria-label="criar nova lista">+</button>
    <button v-else-if="makeTask == 'task'" class="btn create" aria-label="criar nova task">+</button>
</template>

<script>

export default {
    props: {
        makeTask: {type: String, required: true}
    }
};
</script>

<style>

.btn {
 cursor: pointer;
 background: 0;
 border: 0;
 padding: 0;
 color: inherit;
}

.btn.create{
    font-size: 1.5rem;
    font-weight: 900;
    margin-right: 0.25em;
    transition: opacity 150ms ease-in;
}

.btn.create:hover{
    opacity: 0.7;
}
</style>
