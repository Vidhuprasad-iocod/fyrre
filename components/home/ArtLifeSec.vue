<script setup>

import gsap from 'gsap'

const newsItems = ['Lorem ipsum dolor sit amet, consectetur adipiscing elit +++',
                    'Lorem ipsum dolor sit amet, consectetur adipiscing elit +++',
                    "Lorem ipsum dolor sit amet, consectetur adipiscing elit +++",

                ]

onMounted( () => {
    gsap.to('#titleName', {
        opacity: 1,
        y:0,
        duration: 1,
        ease: 'power2.out'
    })

    gsap.fromTo('#newsTracker',
    {   x:'100%'},
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
    <div class="mx-20 flex flex-col">
        <img id="titleName" class="homeImage my-12 relative opacity-0 translate-y-40" src="/assets/home/artLifeSec/artLife.svg" alt="image...">
        <div class="flex gap-2 p-5 mb-[4.5rem] max-md:overflow-scroll bg-black text-white text-center text-sm">
            <h4 class="font-semibold text-base">News Ticker+++</h4>
            <div class="overflow-hidden">
                <div id="newsTracker" class="marquee flex">
                    <template v-for="(news, index) in newsItems" :key="index">
                        {{ news }}&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
                    </template>
                </div>
            </div>
        </div>
        <div class="flex flex-col">
            <div class="flex gap-10 flex-wrap">
                <h1 class="flex-1 font-bold text-8xl">DON'T CLOSE YOUR EYES</h1>
                <div class="flex gap-16 flex-col flex-1">
                    <p class="text-justify text-lg">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.
                    </p>
                    <div>
                        <div class="flex justify-between">
                            <div class="flex gap-8 justify-start items-center text-sm max-md:gap-4">
                                <div class="max-md:flex max-md:flex-col">
                                    <span class="font-semibold pr-2">Text</span><span>Jakob Gronberg</span>
                                </div>
                                <div class="max-md:flex max-md:flex-col">
                                    <span class="font-semibold pr-2">Date</span><span>16. March 2022</span>
                                </div>
                                <div class="max-md:flex max-md:flex-col">
                                    <span class="font-semibold pr-2">Duration</span><span>1 Min</span>
                                </div>
                            </div>
                            <button class="border border-black px-2 py-1 text-xs rounded-xl max-sm:p-0 transition duration-500 hover:bg-black hover:text-white">LABEL</button>
                        </div>
                    </div>
                </div>
            </div>
            <div class="my-12">
                <img src="/assets/magazine/dont-close-your-eyes.webp" alt="image...">
            </div>
        </div>
    </div>
</template>