<template>
    <form v-if="makeTask == 'list'">
        <AllTaskInput makeTask="list"/>
        <AllTaskButton makeTask="list"/>
    </form>
        <form v-else-if="makeTask == 'task'">
        <AllTaskInput makeTask="task"/>
        <AllTaskButton makeTask="task"/>
    </form>
</template>

<script>

import AllTaskInput from '../Inputs/AllTaskInput'
import AllTaskButton from '../Buttons/AllTaskButton'

export default {
    components: {
       AllTaskInput,
       AllTaskButton
    },
    props: {
        makeTask: {type: String, required: true}
    }
};
</script>

<style>

form{
    display: flex;
}

</style>
