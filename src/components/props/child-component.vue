<template>
    <div>
       <div> Title:<label>{{ title }}</label></div>
       <div> Name: <label>{{ name }}</label></div>
       <div>Age: <label>{{ age }}</label></div>
       <div>Graduate: <label>{{ isITGraduate }}</label></div>
    </div>
</template>
<script>
export default {
    name: 'child-component',
    props:{
        title:{
            type: String,
            requied: true,
            default: 'Vue 3 Learner'
        },
        name: String,
        age: Number,
        isITGraduate: Boolean
    }
}
</script>
<style>

</style>