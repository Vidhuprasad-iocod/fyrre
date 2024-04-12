<script setup>

defineComponent({
  name: ['RiArrowRightLine','IconoirArrowDownRight']
});


const magazineData = [
    {
        id: 1,
        title: 'Hope dies last',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        image: '/assets/magazine/hope-dies-last.webp'
    },
    {
        id: 2,
        title: 'The best art museums',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        image: '/assets/magazine/the-best-art-museums.webp'
    },
    {
        id: 3,
        title: 'The devil is the details',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        image: '/assets/magazine/the-devil-is-the-details.webp'
    },
    {
        id: 4,
        title: 'An inde­struc­tible hope',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        image: '/assets/magazine/indestructible-hope.webp'
    },
    {
        id: 5,
        title: 'Street art festival',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        image: '/assets/magazine/street-art-festival.webp'
    },
    {
        id: 6,
        title: 'Through the eyes of street artists',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        image: '/assets/magazine/chains-of-our-lives.webp'
    },
]

const popularMagazine = [
    {
        id: 1,
        title: 'Street art festival',
        text: 'Cristofer Vaccaro'
    },
    {
        id: 2,
        title: 'Hope dies last',
        text: 'Anne Henry'
    },
    {
        id: 3,
        title: 'Artists who want to rise above',
        text: 'Anna Nielsen'
    },
]

</script>



<template>
    <div class="flex max-md:flex-wrap gap-24 mx-20">
        <div class="flex-2 flex flex-col">
            <div v-for="(item, index) in magazineData" :key="index" :class="{'border-b border-black' : index != magazineData.length-1}" class="flex gap-12 max-lg:flex-wrap pb-12 mb-12">
                <div :style="`background-image:url('${item.image}')`" class="w-60 h-60 bg-cover bg-center duration-300 hover:scale-105">
                    <NuxtLink to="/magazine">
                        <div  class="h-60 w-60"></div>
                    </NuxtLink>
                </div>
                <div class="flex gap-20 flex-col justify-between">
                    <div class="flex flex-col gap-3">
                        <h2 class="text-3xl font-semibold">{{ item.title }}</h2>
                        <p class="text-justify">
                            {{ item.content }}
                        </p>
                    </div>
                    <div>
                        <div class="flex justify-between">
                            <div class="flex gap-6 justify-start items-center text-sm max-md:gap-2">
                                <div>
                                    <span class="font-semibold pr-2">Text</span><span>Jakob Gronberg</span>
                                </div>
                                <div>
                                    <span class="font-semibold pr-2">Date</span><span>16. March 2022</span>
                                </div>
                                <div>
                                    <span class="font-semibold pr-2">Read</span><span>1 Min</span>
                                </div>
                            </div>
                            <button class="border border-black px-2 py-1 text-xs rounded-3xl uppercase hover:text-white hover:bg-black duration-500">art</button>
                        </div>
                    </div>
                </div>
            </div>
            <div>
                <NuxtLink to="/magazine" class="font-semibold flex gap-2 items-center">ALL ARTICLES
                    <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24">
		                <path fill="black" d="m16.172 11l-5.364-5.364l1.414-1.414L20 12l-7.778 7.778l-1.414-1.414L16.172 13H4v-2z" />
	                </svg>
                </NuxtLink>    
            </div>
        </div>
        <div class="flex gap-16 flex-col">
            <div>
                <h6 class="mb-2 font-semibold">PRINTMAGAZINE</h6>
                <h2 class="mb-8 text-5xl font-semibold">03/2022</h2>
                <div class="pb-4 relative">
                    <img src="/assets/home/articleSec/magazin-cover.webp" alt="image...">
                    <div class="uppercase text-white font-semibold text-8xl absolute top-4 left-9 flex flex-col gap-24 duration-300 hover:scale-105">
                        <div>
                            <h6>fyrre</h6>
                            <h6 class="text-2xl relative left-1">magazine</h6>
                        </div>
                        <div class="flex flex-col gap-4">
                            <div class="rounded-full bg-[#ECC584] uppercase text-white text-xs h-32 w-32 flex justify-center items-center">
                                <div class="flex flex-col items-center text-center">
                                    <h6>Exclusive</h6>
                                    <h6 class="text-base font-semibold leading-none mt-2">Jacob Gronberg</h6>
                                    <div class="border border-white w-5 my-2"></div>
                                    <h6>Interview</h6>
                                </div>
                            </div>
                            <div class="flex justify-between h-10">
                                <h6 class="text-2xl font-semibold h-fit">03/2022</h6>
                                <svg class="relative top-[-50px]" xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24">
	                            	<path fill="none" stroke="white" stroke-linecap="round" stroke-linejoin="round" stroke-width="1" d="m6 6l13 13m0 0V6.52M19 19H6.52" />
	                            </svg>
                            </div>
                        </div>
                    </div>
                </div>
                <button class="text-sm font-medium text-white bg-black py-2 px-4 hover:shadow-lg">BUTTON</button>
            </div>
            <div>
                <h6 class="mb-8 font-semibold">MOST POPULAR</h6>
                <div v-for="(item, index) in popularMagazine" :key="index" :class="{'border-b border-black pb-6 mb-6' : index != popularMagazine.length-1}" class="flex flex-col">
                    <div class="flex gap-10">
                        <span class="font-semibold text-2xl">0{{ item.id }}</span>
                        <div class="flex flex-col gap-3">
                            <h3 class="font-semibold text-2xl">{{ item.title }}</h3>
                            <p class="text-sm"><span class="font-semibold pr-2">Text</span>{{ item.title }}</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="p-7 bg-[#F8F8F8] flex flex-col gap-4">
                <div class="flex flex-col gap-2">
                    <h6 class="font-semibold">NewsLetter</h6>
                    <h1 class="text-3xl font-semibold">Design News to your inbox</h1>
                </div>
                <div class="flex flex-col gap-3">
                    <input class="px-4 py-3" type="email" name="" id="" placeholder="Email">
                    <div class="flex justify-end">
                        <button class="text-white text-sm font-medium bg-black px-6 py-4 uppercase">sign up</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>