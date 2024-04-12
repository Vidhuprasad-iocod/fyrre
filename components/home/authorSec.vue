<script setup>

const authorsData = [
    {
        id: 1,
        name: 'Jakob Grønberg',
        image: '/assets/authors/jakob-grønberg.webp',
        job: 'Artist',
        city: 'Berlin'
    },
    {
        id: 2,
        name: 'Louise Jensen',
        image: '/assets/authors/louise-jensen.webp',
        job: 'Artist',
        city: 'Stockholm'
    },
    {
        id: 3,
        name: 'Anne Henry',
        image: '/assets/authors/anne-henry.webp',
        job: 'Photograph',
        city: 'New York'
    },
    {
        id: 4,
        name: 'Anna Nielsen',
        image: '/assets/authors/anna-nielsen.webp',
        job: 'Columnists',
        city: 'Copenhagen'
    },
    {
        id: 5,
        name: 'Jane Cooper',
        image: '/assets/authors/jane-cooper.webp',
        job: 'Artist',
        city: 'Berlin'
    },
    {
        id: 6,
        name: 'Cristofer Vaccaro',
        image: '/assets/authors/cristofer-vaccaro.webp',
        job: 'Artist',
        city: 'Lisbon'
    }
]

</script>



<template>
    <div class="flex flex-col gap-5 mx-20 my-20">
        <div class="flex flex-wrap justify-between items-center border-t border-black pt-10">
            <h1 class="text-8xl font-semibold max-md:text-5xl">AUTHORS</h1>
            <NuxtLink to="/authors" class="font-semibold flex gap-2 items-center">ALL AUTHORS
                <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 24 24">
		            <path fill="black" d="m16.172 11l-5.364-5.364l1.414-1.414L20 12l-7.778 7.778l-1.414-1.414L16.172 13H4v-2z" />
	            </svg>
            </NuxtLink>
        </div>
        <div class="grid grid-cols-2 border border-gray-100 max-md:grid-cols-1 my-20">
           <div v-for="(item, index) in authorsData" :key="index" class="flex flex-wrap gap-10 items-center p-5  border border-black">
                <NuxtLink to="/authors">
                    <img class="w-[150px] h-[150px] rounded-full hover:scale-105 duration-300" :src="item.image" alt="image...">
                </NuxtLink>
                <div class="flex flex-col gap-5">
                    <h3 class="text-3xl font-semibold">{{ item.name }}</h3>
                    <div class="flex gap-8 justify-start items-center text-sm">
                        <div>
                            <span class="font-semibold pr-2">Job</span><span>{{ item.job }}</span>
                        </div>
                        <div>
                            <span class="font-semibold pr-2">City</span><span>{{ item.city }}</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>