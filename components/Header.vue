<script setup>
import gsap from 'gsap'

const magazineAnimation = (isHovering) => {
    gsap.to('#magazineBtn', {
        rotationX: isHovering ? 360 : 0,
        backgroundColor: isHovering ? 'black' : 'white',
        color: isHovering ? 'white' : 'black',
        duration: 0.4,
        ease: 'linear'
    })
}

const authorsAnimation = (isHovering) => {
    gsap.to('#authorsBtn', {
        rotationX: isHovering ? 360 : 0 ,
        backgroundColor: isHovering ? 'black' : 'white',
        color: isHovering ? 'white' : 'black',
        duration: 0.4,
        ease: 'linear'
    })

}

const podcastAnimation = (isHovering) => {
    gsap.to('#podcastBtn', {
        rotationX: isHovering ? 360 : 0 ,
        backgroundColor: isHovering ? 'black' : 'white',
        color: isHovering ? 'white' : 'black',
        duration: 0.4,
        ease: 'linear'
    })

}

</script>


<template>
    <header class="mx-20 mt-16">
        <div class=" flex flex-wrap justify-between items-center border-b border-black pb-4">
            <NuxtLink to="/">
                <img src="/assets/header/fyrre-magazine.svg" alt="image...">
            </NuxtLink>
            <ul class="flex flex-wrap gap-5 items-center">
                <li class="flex" @mouseenter="magazineAnimation(true)" @mouseleave="magazineAnimation(false)">
                    <nuxt-link class="px-3 py-1 rounded" id="magazineBtn" to="/magazine">Magazine</nuxt-link>
                </li>
                <li class="flex" @mouseenter="authorsAnimation(true)" @mouseleave="authorsAnimation(false)">
                    <nuxt-link class="px-3 py-1 rounded" id="authorsBtn" to="/authors">Authors</nuxt-link>
                </li>
                <li class="flex" @mouseenter="podcastAnimation(true)" @mouseleave="podcastAnimation(false)">
                    <nuxt-link class="px-3 py-1 rounded" id="podcastBtn" to="/podcasts">Podcast</nuxt-link>
                </li>
                <li class="border border-black w-4"></li>
                <li>
                    <social-media color="black"/>
                </li>
            </ul>
        </div>
    </header>
</template>


