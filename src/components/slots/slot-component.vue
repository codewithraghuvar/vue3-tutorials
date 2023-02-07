<template>
    <div>
        <cardData>
            This is my Card text
        </cardData>

        <cardData>
            <h1>My page </h1>
            This is my Card content
        </cardData>

        https://picsum.photos/seed/picsum/200/300
        <cardContainer>
            <template v-slot:header>
                   This is header
            </template>
            <template v-slot:default>
                This is content
            </template>
            <template v-slot:footer>
                This is footer
            </template>
        </cardContainer>
        
    </div>
</template>
<script>
import cardData from './card-data.vue';
import cardContainer from './card-container.vue';
export default {
    name: 'slot-component',
    components:{
        cardData,
        cardContainer
    }
}
</script>
<style>
</style>