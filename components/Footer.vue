<script setup>
import gsap from 'gsap'

const newsLatter = [
    'Newsletter+++',
    'Newsletter+++',
    'Newsletter+++',
    'Newsletter+++',
    'Newsletter+++',
    'Newsletter+++',
    'Newsletter+++',
    'Newsletter+++',
    'Newsletter+++',
    'Newsletter+++'
]

onMounted( () => {
    gsap.fromTo('#newsLatter', 
    {   x: '100%'},
    {
        x: '-100%',
        duration: 20,
        repeat: Infinity,
        ease: 'linear'
    }
)
})

</script>


<template>
    <footer class="bg-black text-white box-border">
        <ul class="flex justify-between text-lg font-semibold p-5 overflow-hidden">
            <li id="newsLatter" class="marquee flex">
                <template v-for="(news, index) in newsLatter" :key="index">
                    {{ news }}&nbsp;&nbsp;&nbsp;
                </template>
            </li>
        </ul>
        <div class="flex gap-20 flex-col px-20 pb-6 mt-20">
            <div class="flex flex-wrap justify-between my-10 items-center max-md:gap-5">
                <h1 class="text-7xl font-semibold">DESIGN NEWS TO <br> YOUR INBOX</h1>
                <form class="flex flex-wrap gap-3 h-fit" action="">
                    <input class="flex-1 text-black pl-4 md:w-[20dvw]" type="email" name="" id="" placeholder="Email">
                    <button class="bg-white text-black px-6 py-4 text-sm font-semibold">SIGN UP</button>
                </form>
            </div>
            <div class="flex flex-wrap gap-20 flex-col">
                <div class="flex flex-wrap">
                    <div class="flex-1">
                        <h6 class="font-semibold text-xl">FYRRE MAGAZINE</h6>
                    </div>
                    <div class="flex flex-wrap gap-20 flex-1 pt-5 font-light text-base">
                        <ul class="flex-1 flex flex-col gap-4">
                            <li>Art</li>
                            <li>Design</li>
                            <li>Architecture</li>
                        </ul>
                        <ul class="flex-1 flex flex-col gap-4">
                            <li>Magazine</li>
                            <li>Podcast</li>
                            <li>Authors</li>
                        </ul>
                        <ul class="flex-1 flex flex-col gap-4">
                            <li>Styleguide</li>
                            <li>Licensing</li>
                            <li>Changelog</li>
                        </ul>
                    </div>
                </div>
                <div class="flex justify-between">
                    <p class="text-sm font-light">© Made by Pawel Gola -  Powered by Webflow</p>
                    <social-media color="white"/>
                </div>
            </div>
        </div>
    </footer>
</template>


