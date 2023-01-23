<script>
import ProductCard from './products/ProductCard.vue';
export default {
    name: "AppMain",
    components: { ProductCard },
    props: {
        products: Array
    }
};
</script>

<template>
    <main>
        <!-- main-content -->
        <section id="products">
            <div class="container">
                <h3>Current Series</h3>
                <div class="card-container">
                    <product-card v-for="product in products" :key="product.series" :product="product"></product-card>
                    <a href="#">Load More</a>
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
//importo file scss
@use '../assets/scss/partials/mixins' as *;
@use '../assets/scss/partials/variables' as *;

#products {
    padding: 30px 0;
    min-height: 300px;
    color: white;
    background-color: $almostblack;

    h3 {
        @include main-buttons;
        display: inline-block;
    }

    .card-container {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        margin-top: 20px;

        .product-card {
            flex-basis: calc(100% / 6);
        }

        a {
            @include main-buttons;
            color: white;
        }
    }
}
</style>