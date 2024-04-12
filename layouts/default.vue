<template>
    <div>
        <Header />
        <slot />
        <Footer />
    </div>
</template>


<script setup>
useHead({
    titleTemplate : 'Fyrre',
})

</script>

<style scoped>
html{
    scroll-behavior: smooth;
}
</style>

