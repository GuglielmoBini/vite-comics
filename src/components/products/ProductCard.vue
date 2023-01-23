<script>
export default {
    name: "ProductCard",
    props: {
        product: Object
    }
}
</script>

<template>
    <div class="product-card">
        <figure>
            <a href="#"><img :src="product.thumb" :alt="product.series"></a>
        </figure>
        <figcaption>{{ product.series }}</figcaption>
    </div>
</template>

<style lang="scss" scoped>
.product-card {
    padding: 15px;

    figure img {
        display: block;
        width: 150px;
        height: 150px;
        object-fit: cover;
        object-position: top;
    }

    figcaption {
        margin-top: 15px;
        text-transform: uppercase;
    }
}
</style>