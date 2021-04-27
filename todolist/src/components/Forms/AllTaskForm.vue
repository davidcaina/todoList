<template>
    <form action="">
        <AllTaskInput/>
        <AllTaskButton/>
    </form>
</template>

<script>

import AllTaskInput from '../Inputs/AllTaskInput'
import AllTaskButton from '../Buttons/AllTaskButton'

export default {
    components: {
       AllTaskInput,
       AllTaskButton
    }
};
</script>

<style scoped>

</style>
