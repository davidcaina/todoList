<template>
    <li v-if="isActive == 'active'" :class="activeList">
        {{nomeElemento}}
    </li>
        <li v-else class="">
        {{nomeElemento}}
    </li>
</template>

<script>

export default {
    props:{
        nomeElemento: String,
        isActive: String
    },
    data(){
        return{
            activeList: "active-list",
        }
    }
};
</script>

<style>

.active-list{
    font-weight: bold;
}
</style>
