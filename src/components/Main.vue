<template>
    <div class="main-container">
        <div class="container">
         <Card v-for="product in products" :key="product.id" :product="product"/>
        </div>
    </div>
</template>

<script>

import Card from './Card.vue'

export default {
    name: 'Main',
    components: {
        Card
    },
    props: ['products'],
    data: function() {
        return {
            
        }
    }
}
</script>


<style lang="scss" scoped>

    .main-container {
        background: url("../assets/fondo-pag-speciali.jpg");

        .container {
            display: flex;
            flex-wrap: wrap;
        }

    }

</style>