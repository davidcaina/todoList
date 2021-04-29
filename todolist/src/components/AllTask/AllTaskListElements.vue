<template>
    <li v-if="isActive == 'active'" :class="activeList">
        {{nomeElemento}}
    </li>
        <li v-else :class="clickable">
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
            activeList: "active-list list-name",
            clickable: "list-name"
        }
    }
};
</script>

<style>

.active-list{
    font-weight: bold;
}

.list-name{
    cursor: pointer;
}
.list-name:hover{
    opacity: 0.7;
}
</style>
