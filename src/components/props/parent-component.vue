<template>
    <div>
        <childComponent 
        :title="'Vue3 new learner'"
        :name="'Raghuvar'"
        :age="30"
        :isITGraduate="true"/>
    </div>
</template>
<script>
import childComponent from './child-component.vue';
export default {
    name: 'parent-component',
    components:{
        childComponent 
    }
}
</script>
<style>

</style>