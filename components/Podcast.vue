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

const itemPassing = (item) =>{
    console.log(item.id);
}




</script>



<template>
    <div class="mx-20 my-10">
        <div class="mb-8">
            <img src="/assets/podcast/podcast.svg" alt="image...">
        </div>
        <div class="pt-24">
            <div v-for="(item, index) in podcast" :key="index" :class="{'border-b border-black': index !== podcast.length-1}" class="grid grid-cols-10 gap-10 items-center pb-20 mb-20">
                <h3 class="col-span-1 text-2xl font-semibold">0{{ item.id }}</h3>
                <img class="col-span-2" :src="item.image" alt="image...">
                <h2 class="col-span-3 text-3xl font-semibold">{{ item.title }}</h2>
                <div class="col-span-3 flex gap-8 justify-end items-center text-sm max-md:gap-2">
                    <div>
                        <span class="font-semibold pr-2">Date</span><span>16. March 2022</span>
                    </div>
                    <div>
                        <span class="font-semibold pr-2">Duration</span><span>1 Min</span>
                    </div>          
                </div>
                <NuxtLink @click="itemPassing(item)" to="/podcasts/podcastPost" class="col-span-1 text-base font-semibold flex gap-2 items-center uppercase justify-end">
                    Listen
                     <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 24 24">
		                 <path fill="black" d="m16.172 11l-5.364-5.364l1.414-1.414L20 12l-7.778 7.778l-1.414-1.414L16.172 13H4v-2z" />
	                 </svg>
                </NuxtLink>  
            </div>
        </div>
    </div>
</template>