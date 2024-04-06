<script setup>

const authors = [
    {
        image: '/assets/home/authorSec/jakob.svg',
        name: 'Jakob Grønberg'
    },
    {
        image: '/assets/home/authorSec/louise.svg',
        name: 'Louise Jensen'
    },
    {
        image: '/assets/home/authorSec/anne.svg',
        name: 'Anne Henry'
    },
    {
        image: '/assets/home/authorSec/anna.svg',
        name: 'Anna Nielsen'
    },
    {
        image: '/assets/home/authorSec/jane.svg',
        name: 'Jane Cooper'
    },
    {
        image: '/assets/home/authorSec/cristofer.svg',
        name: 'Cristofer Vaccaro'
    }
]


</script>




<template>
    <div class="mx-20 my-10">
        <div class="pb-10">
            <img src="/assets/authors/Authors.svg" alt="image...">
        </div>
        <div class="my-20">
            <div v-for="(item, index) in authors" :key="index" :class="{'border-b border-black': index !== authors.length-1}" class="flex justify-between  pb-10 mb-10">
                <div class="flex flex-wrap gap-10 items-center">
                    <img :src="item.image" alt="image...">
                    <h3 class="text-3xl font-semibold">{{ item.name }}</h3>
                </div>
                <div class="flex gap-20 justify-start items-center text-sm">
                    <div>
                        <span class="font-semibold pr-2">Job</span><span>Artist</span>
                    </div>
                    <div>
                        <span class="font-semibold pr-2">City</span><span>Berlin</span>
                    </div>
                    <NuxtLink class="uppercase font-semibold flex items-center gap-2" to="/authors/authorsPost">
                        about
                        <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 24 24">
		                    <path fill="black" d="m16.172 11l-5.364-5.364l1.414-1.414L20 12l-7.778 7.778l-1.414-1.414L16.172 13H4v-2z" />
	                    </svg>
                    </NuxtLink>
                </div>
            </div>
        </div>
    </div>
</template>