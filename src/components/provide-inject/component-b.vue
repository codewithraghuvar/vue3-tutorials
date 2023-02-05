<template>
    <div>
    Component b
    <componentC/>
    </div>
</template>
<script>
import componentC from './component-c.vue';
export default {
    name: 'component-b',
    components:{
        componentC
    }
}
</script>
<style>
</style>