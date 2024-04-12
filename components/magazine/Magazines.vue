<script setup>

const data = [
    {
        _id: 0,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/hope-dies-last.webp',
        title: 'Hope dies last',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 1,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/dont-close-your-eyes.webp',
        title: 'Don’t close your eyes',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 2,
        date: '16. March 2022',
        type: 'Sculptures',
        image: '/assets/magazine/the-best-art-museums.webp',
        title: 'The best art museums',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 3,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/the-devil-is-the-details.webp',
        title: 'The devil is the details',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 4,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/indestructible-hope.webp',
        title: 'An indestructible hope',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 5,
        date: '16. March 2022',
        type: 'street art',
        image: '/assets/magazine/street-art-festival.webp',
        title: 'Street art festival',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 6,
        date: '16. March 2022',
        type: 'Sculptures',
        image: '/assets/magazine/chains-of-our-lives.webp',
        title: 'The chains of our lives',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 7,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/through-the-eyes-of-street-artists.webp',
        title: 'Through the eyes of street artists',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 8,
        date: '16. March 2022',
        type: 'street art',
        image: '/assets/magazine/artists-who-want-to-rise-above.webp',
        title: 'Artists who want to rise above',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 9,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/secret-garden.webp',
        title: 'Secret garden',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 10,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/getting-real.webp',
        title: 'Getting real',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 11,
        date: '16. March 2022',
        type: 'street art',
        image: '/assets/magazine/most-coloful-places.webp',
        title: 'Most coloful places',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 12,
        date: '16. March 2022',
        type: 'street art',
        image: '/assets/magazine/keep-on-smiling.webp',
        title: 'Keep on Smiling',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 13,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/history-of-paper.webp',
        title: 'History of Paper',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 14,
        date: '16. March 2022',
        type: 'Sculptures',
        image: '/assets/magazine/how-are-you.webp',
        title: 'How are you, really?',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 15,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/beauty-of-colors.webp',
        title: 'Beauty of Colors',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 16,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/colorful-future.webp',
        title: 'Colorful Future',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        _id: 17,
        date: '16. March 2022',
        type: 'Sculptures',
        image: '/assets/magazine/only-in-your-heart.webp',
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
                <div :style="`background-image: url('${item.image}')`" class="w-[380px] h-[380px] bg-cover bg-center duration-300 hover:scale-105 hover:shadow-xl"></div>
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