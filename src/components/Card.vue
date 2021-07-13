<template>
    <div class="product-card">
        <img :src="product.src"/>
        <div class="product-name">{{product.titolo}}</div>
    </div>
    
</template>


<script>
export default {
    name: 'Card',
    props: ['product']
}
</script>

<style lang="scss" scoped>

    .product-card {
        width: calc(100% / 3);
        border-radius: 15px;
        background: #fff;
        padding: 20px 0;

        img {
            width: 100%;
        }

        .product-name {
            font-size: 20px;
            text-align: center;
            font-weight: bold;
        }
    }

</style>