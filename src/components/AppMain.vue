<script>
export default {
    name: "AppMain"
}
</script>

<template>
    <main>
        <section id="main-content">
            <h2>Content goes here</h2>
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixins' as *;
@use '../assets/scss/partials/variables' as *;

#main-content {
    @include flex-center;
    min-height: 300px;
    color: white;
    background-color: $almostblack;
}
</style>