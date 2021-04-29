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

<style>

.custom-checkbox{

    --size: .75em;

    display: inline-block;
    width: var(--size);
    height: var(--size);
    cursor: pointer;
    border: 2px solid currentColor;
    border-radius: 50%;
    margin-right: var(--size);

    transform: scale(1);
    transition: transform 200ms ease-in-out;
}

.task:hover .custom-checkbox, [type="checkbox"]:focus + label .custom-checkbox{
    transform: scale(1.2);
    color: var(--primary-color)
}

[type="checkbox"]:checked + label .custom-checkbox{
    background: var(--primary-color);
    border-color: var(--primary-color);
    box-shadow: inset 0 0 0px 1px white;
}

.task label{
    display: flex;
    align-items: center;
    position: relative;
    margin-bottom: 1.25em;
}

.task label::after{
    content: "";
    position: absolute;
    right: 0;
    left: 0;
    bottom: -50%;
    height: 1px;
    background: currentColor;
    opacity: 0.2;
}

</style>
