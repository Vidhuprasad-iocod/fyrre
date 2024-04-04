<template>
    <div>
        <Header />
        <slot />
        <Footer />
    </div>
</template>


<script setup>
useHead({
    titleTemplate : '%s - Fyrre',
})

</script>

<style scoped>
html{
    scroll-behavior: smooth;
}
</style>

