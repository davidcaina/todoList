<template>
    <div class="task"> 
        <input type="checkbox" :id=taskId>
        <label :for=taskId>
            <span class="custom-checkbox"></span>
             {{taskMessage}}
        </label>
    </div>
</template>

<script>

export default {
    props:{
        taskId: String,
        taskMessage: String
    }
};
</script>

<style scoped>

</style>
