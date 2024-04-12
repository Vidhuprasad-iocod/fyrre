<script setup>

const podcastDatas = [
    {
        id: 1,
        title: 'The Problem of today’s cultural development',
        duration: '1h 20 Min',
        image: '/assets/podcast/problem-of-todays-culture.webp'
    },
    {
        id: 2,
        title: 'The hidden messages of Jack Nielson',
        duration: '60 Min',
        image: '/assets/podcast/jack-nielson.webp'
    },
    {
        id: 3,
        title: 'Behind the scenes of the street art culture',
        duration: '45 Min',
        image: '/assets/podcast/street-art.webp'
    }
]

</script>


<template>
    <div class="mx-20 my-24">
        <div class="flex flex-wrap justify-between items-center border-t border-black pt-12 mb-24">
            <h1 class="text-8xl font-semibold max-md:text-5xl">PODCAST</h1>
            <NuxtLink to="/podcasts" class="font-semibold flex gap-2 items-center uppercase">all episodes
                <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24">
		            <path fill="black" d="m16.172 11l-5.364-5.364l1.414-1.414L20 12l-7.778 7.778l-1.414-1.414L16.172 13H4v-2z" />
	            </svg>
            </NuxtLink>
        </div>
        <div class="flex flex-wrap">
            <div v-for="(items, index) in podcastDatas" :key="index"  class="flex flex-col gap-4 p-8 border border-black flex-1">
                <img class="w-[408px] h-[408px] hover:scale-105 hover:shadow-xl duration-300" :src="items.image" alt="image...">
                <div class="flex flex-col gap-10">
                    <h3 class="text-3xl font-semibold">{{ items.title }}</h3>
                    <div class="flex gap-8 justify-start items-center text-sm">
                        <div>
                            <span class="font-semibold pr-2">Date</span><span>16.06.2022</span>
                        </div>
                        <div>
                            <span class="font-semibold pr-2">Duration</span><span>{{ items.duration }}</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>