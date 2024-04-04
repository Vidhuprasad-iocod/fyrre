<script setup>

const podcast = [
    {
        id: 5,
        image: '/assets/podcast/podcast-cover05.svg',
        title: 'The Problem of today’s cultural development'
    },
    {
        id: 4,
        image: '/assets/podcast/podcast-cover04.svg',
        title: 'The hidden messages of Jack Nielson'
    },
    {
        id: 3,
        image: '/assets/podcast/podcast-cover03.svg',
        title: 'Behind the scenes of the street art culture'
    },
    {
        id: 2,
        image: '/assets/podcast/podcast-cover02.svg',
        title: 'The art of movement'
    },
    {
        id: 1,
        image: '/assets/podcast/podcast-cover01.svg',
        title: '10 artists your should definitely know'
    }
    
]


</script>



<template>
    <div class="mx-20 my-10 flex flex-col gap-20">
        <h1 class="text-[17dvw] leading-[14dvw] font-bold text-center w-full my-5 mb-20 uppercase tracking-[1.8dvw]">
            podcast
        </h1>
        <div v-for="(item, index) in podcast" :key="index" class="flex flex-col gap-20">
            <div class="flex justify-between">
                <div class="flex items-center gap-16">
                    <h3 class="text-2xl font-semibold">{{ item.id }}</h3>
                    <img src="/assets/podcast/podcast-cover05.svg" alt="">
                    <h2 class="text-3xl font-semibold">{{ item.title }}</h2>
                </div>
                <div class="flex items-center">
                    <div class="flex gap-8 justify-start items-center text-sm max-md:gap-2">
                        <div class="lg:flex-2">
                            <span class="font-semibold pr-2">Date</span><span>16. March 2022</span>
                        </div>
                        <div class="lg:flex-1">
                            <span class="font-semibold pr-2">Duration</span><span>1 Min</span>
                        </div>
                        <a class="text-base font-semibold flex gap-2 items-center uppercase" href="">listen
                            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24">
		                        <path fill="black" d="m16.172 11l-5.364-5.364l1.414-1.414L20 12l-7.778 7.778l-1.414-1.414L16.172 13H4v-2z" />
	                        </svg>
                        </a>            
                    </div>
                </div>
            </div>
            <div class="border border-black"></div>
        </div>
    </div>
</template>