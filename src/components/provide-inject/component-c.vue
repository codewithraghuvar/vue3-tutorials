<template>
    <div>
        Component C
       username : {{ username }}
    </div>
</template>
<script>
export default {
    name: 'component-c',
    inject:['username']
}
</script>
<style>
</style>