<script setup>

const data = [
    {
        _id: 0,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/hope.svg',
        title: 'Hope dies last',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 1,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/eyes.svg',
        title: 'Don’t close your eyes',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 2,
        date: '16. March 2022',
        type: 'Sculptures',
        image: '/assets/magazine/artMuseum.svg',
        title: 'The best art museums',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 3,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/devil.svg',
        title: 'The devil is the details',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 4,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/indestructibleHope.svg',
        title: 'An indestructible hope',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 5,
        date: '16. March 2022',
        type: 'street art',
        image: '/assets/magazine/streetArt.svg',
        title: 'Street art festival',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 6,
        date: '16. March 2022',
        type: 'Sculptures',
        image: '/assets/magazine/chainOfLives.svg',
        title: 'The chains of our lives',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 7,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/streetArtist.svg',
        title: 'Through the eyes of street artists',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 8,
        date: '16. March 2022',
        type: 'street art',
        image: '/assets/magazine/riseAbove.svg',
        title: 'Artists who want to rise above',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 9,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/SecretGarden.svg',
        title: 'Secret garden',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 10,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/real.svg',
        title: 'Getting real',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 11,
        date: '16. March 2022',
        type: 'street art',
        image: '/assets/magazine/colorfulPlace.svg',
        title: 'Most coloful places',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 12,
        date: '16. March 2022',
        type: 'street art',
        image: '/assets/magazine/smiling.svg',
        title: 'Keep on Smiling',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 13,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/historyOfPaper.svg',
        title: 'History of Paper',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 14,
        date: '16. March 2022',
        type: 'Sculptures',
        image: '/assets/magazine/howRU.svg',
        title: 'How are you, really?',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 15,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/colors.svg',
        title: 'Beauty of Colors',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 16,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/colorfulFuture.svg',
        title: 'Colorful Future',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 17,
        date: '16. March 2022',
        type: 'Sculptures',
        image: '/assets/magazine/heart.svg',
        title: 'Only in Your Heart',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    }
]



</script>




<template>
    <div class="grid grid-cols-3">
        <div v-for="(item, index) in data" :key="index" class="p-10 flex flex-col gap-5 border border-black">
            <div class="flex justify-between">
                <p class="text-sm">{{item.date }}</p>
                <label class="text-xs uppercase border border-black rounded-3xl px-3 py-2" for="">{{item.type }}</label>
            </div>
            <NuxtLink to="/magazine/magazinePost">
                <img :src="item.image" alt="image...">
            </NuxtLink>
            <div class="flex gap-20 flex-col justify-between">
            <div class="flex flex-col gap-2">
                <h2 class="text-3xl font-semibold">{{item.title }}</h2>
                <p class="text-justify">{{item.content }}</p>
            </div>
            <div>
                <div class="flex justify-between">
                    <div class="flex gap-8 justify-start items-center text-sm">
                        <div>
                            <span class="font-semibold pr-2">Text</span><span>{{item.text }}</span>
                        </div>
                        <div>
                            <span class="font-semibold pr-2">Duration</span><span>{{item.duration }}</span>
                        </div>
                    </div>
                </div>
            </div>
            </div>
        </div>
    </div>
</template>