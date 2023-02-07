<template>
    <div class="card-wrapper">
        <div class="card-header"> 
            <slot name="header"></slot> 
        </div>
        <div class="card-content">
            <!-- default slot-->
            <slot></slot>
        </div>
        <div class="card-footer"> 
            <slot name="footer"></slot>
        </div>
    </div>
</template>
<script>
    export default {
        name: 'card-data'
    }
</script>
<style>
</style>