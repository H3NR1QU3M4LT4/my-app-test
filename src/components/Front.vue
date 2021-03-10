<template>
    <header>
        <h1>{{title}}</h1>
        <Button text="Add task" color="green"/>
        <Button text="Add task" color="blue"/>
        <Button text="Add task" color="red"/>
    </header>
</template>

<script>

import Button from './Button.vue'

export default {
    name: 'Front',
    props: ['title'],
    //or props
    //props:{
    //  title: String,
    //},
    components: {
        Button
    }
}
</script>

<style scoped>
    Front {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
    }
</style>