<template>
    <div>
        Component Second
       username : {{ username }}
    </div>
</template>
<script>
export default {
    name: 'component-second',
    inject:['username']
}
</script>
<style>
</style>