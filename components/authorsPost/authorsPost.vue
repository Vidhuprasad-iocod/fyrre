<script setup>

const articles = [
    {
        title: 'The best art museums',
        image: '/assets/authors/authorsPost/articles/museum.svg'
    },
    {
        title: 'An inde­struc­tible hope',
        image: '/assets/authors/authorsPost/articles/hope.svg'
    },
    {
        title: 'The chains of our lives',
        image: '/assets/authors/authorsPost/articles/lives.svg'
    },
    {
        title: 'Keep on smiling',
        image: '/assets/authors/authorsPost/articles/smiling.svg'
    }
    
]

</script>



<template>
    <div class="mx-20 my-10">
        <div class="flex justify-between mb-10">
            <NuxtLink to="/authors"
                class="col-span-1 text-base font-semibold flex gap-2 items-center uppercase justify-end">
                <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 24 24">
                    <path fill="black"
                        d="M7.828 11H20v2H7.828l5.364 5.364l-1.414 1.414L4 12l7.778-7.778l1.414 1.414z" />
                </svg>
                GO BACK
            </NuxtLink>
            <h3 class="text-3xl font-semibold uppercase">authors</h3>
        </div>
        <div class="py-10 mb-20 mx-32 grid grid-cols-9 gap-24">
            <div class="flex flex-col gap-10 col-span-3">
                <img src="/assets/authors/authorsPost/louise.svg" alt="image..." />
                <div class="pt-10 flex justify-between gap-8 border-t border-black">
                    <h3 class="font-semibold">Follow</h3>
                    <ul class="flex gap-2">
                        <li>
                            <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 24 24">
                                <path :fill="color"
                                    d="M12.001 9a3 3 0 1 0 0 6a3 3 0 0 0 0-6m0-2a5 5 0 1 1 0 10a5 5 0 0 1 0-10m6.5-.25a1.25 1.25 0 0 1-2.5 0a1.25 1.25 0 0 1 2.5 0M12.001 4c-2.474 0-2.878.007-4.029.058c-.784.037-1.31.142-1.798.332a2.886 2.886 0 0 0-1.08.703a2.89 2.89 0 0 0-.704 1.08c-.19.49-.295 1.015-.331 1.798C4.007 9.075 4 9.461 4 12c0 2.475.007 2.878.058 4.029c.037.783.142 1.31.331 1.797c.17.435.37.748.702 1.08c.337.336.65.537 1.08.703c.494.191 1.02.297 1.8.333C9.075 19.994 9.461 20 12 20c2.475 0 2.878-.007 4.029-.058c.782-.037 1.308-.142 1.797-.331a2.91 2.91 0 0 0 1.08-.703c.337-.336.538-.649.704-1.08c.19-.492.296-1.018.332-1.8c.052-1.103.058-1.49.058-4.028c0-2.474-.007-2.878-.058-4.029c-.037-.782-.143-1.31-.332-1.798a2.912 2.912 0 0 0-.703-1.08a2.884 2.884 0 0 0-1.08-.704c-.49-.19-1.016-.295-1.798-.331C14.926 4.006 14.54 4 12 4m0-2c2.717 0 3.056.01 4.123.06c1.064.05 1.79.217 2.427.465c.66.254 1.216.598 1.772 1.153a4.908 4.908 0 0 1 1.153 1.772c.247.637.415 1.363.465 2.428c.047 1.066.06 1.405.06 4.122c0 2.717-.01 3.056-.06 4.122c-.05 1.065-.218 1.79-.465 2.428a4.884 4.884 0 0 1-1.153 1.772a4.915 4.915 0 0 1-1.772 1.153c-.637.247-1.363.415-2.427.465c-1.067.047-1.406.06-4.123.06c-2.717 0-3.056-.01-4.123-.06c-1.064-.05-1.789-.218-2.427-.465a4.89 4.89 0 0 1-1.772-1.153a4.905 4.905 0 0 1-1.153-1.772c-.248-.637-.415-1.363-.465-2.428C2.012 15.056 2 14.717 2 12c0-2.717.01-3.056.06-4.122c.05-1.065.217-1.79.465-2.428a4.88 4.88 0 0 1 1.153-1.772A4.897 4.897 0 0 1 5.45 2.525c.637-.248 1.362-.415 2.427-.465C8.945 2.013 9.284 2 12.001 2" />
                            </svg>
                        </li>
                        <li>
                            <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 24 24">
                                <path :fill="color" fill-rule="evenodd"
                                    d="M22 5.892a8.178 8.178 0 0 1-2.355.635a4.074 4.074 0 0 0 1.8-2.235a8.343 8.343 0 0 1-2.605.981A4.13 4.13 0 0 0 15.85 4a4.068 4.068 0 0 0-4.1 4.038c0 .31.035.618.105.919A11.705 11.705 0 0 1 3.4 4.734a4.006 4.006 0 0 0 1.268 5.392a4.165 4.165 0 0 1-1.859-.5v.05A4.057 4.057 0 0 0 6.1 13.635a4.192 4.192 0 0 1-1.856.07a4.108 4.108 0 0 0 3.831 2.807A8.36 8.36 0 0 1 2 18.184A11.732 11.732 0 0 0 8.291 20A11.502 11.502 0 0 0 19.964 8.5c0-.177 0-.349-.012-.523A8.143 8.143 0 0 0 22 5.892"
                                    clip-rule="evenodd" />
                            </svg>
                        </li>
                        <li>
                            <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 24 24">
                                <path :fill="color" fill-rule="evenodd"
                                    d="M21.7 8.037a4.26 4.26 0 0 0-.789-1.964a2.84 2.84 0 0 0-1.984-.839c-2.767-.2-6.926-.2-6.926-.2s-4.157 0-6.928.2a2.836 2.836 0 0 0-1.983.839a4.225 4.225 0 0 0-.79 1.965a30.146 30.146 0 0 0-.2 3.206v1.5a30.12 30.12 0 0 0 .2 3.206c.094.712.364 1.39.784 1.972c.604.536 1.38.837 2.187.848c1.583.151 6.731.2 6.731.2s4.161 0 6.928-.2a2.844 2.844 0 0 0 1.985-.84a4.27 4.27 0 0 0 .787-1.965a30.12 30.12 0 0 0 .2-3.206v-1.516a30.672 30.672 0 0 0-.202-3.206m-11.692 6.554v-5.62l5.4 2.819z"
                                    clip-rule="evenodd" />
                            </svg>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="flex flex-col gap-20 col-span-6">
                <div class="flex flex-col gap-8">
                    <div>
                        <h6 class="uppercase pb-2 font-semibold">episode 01</h6>
                        <h1 class="uppercase text-[6.4rem] leading-[6rem] font-semibold">
                            Louise Jensen
                        </h1>
                    </div>
                    <p class="text-xl font-medium">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                        eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas
                        dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu
                        felis bibendum ut. Porttitor leo a diam.
                    </p>
                </div>
                <p class="whitespace-pre-line">
                    Porttitor rhoncus dolor purus non enim praesent elementum. Eget dolor morbi non arcu risus quis
                    varius. Posuere ac ut consequat semper viverra nam libero. In ornare quam viverra orci sagittis eu.
                    Tristique risus nec feugiat in fermentum posuere urna nec. Tempus quam pellentesque nec nam aliquam
                    sem et. Convallis a cras semper auctor neque vitae tempus quam pellentesque. Sollicitudin ac orci
                    phasellus egestas tellus rutrum tellus pellentesque. Sed egestas egestas fringilla phasellus
                    faucibus scelerisque eleifend donec pretium. Sit amet porttitor eget dolor morbi non arcu risus.
                    Justo eget magna fermentum iaculis eu non diam phasellus. Sit amet luctus venenatis lectus magna
                    fringilla. Neque vitae tempus quam pellentesque nec nam.
                </p>
            </div>
        </div>
        <div class="flex flex-col gap-10 border-t border-black pt-10 mt-10">
            <h2 class="text-7xl font-semibold">Articles by Louise Jensen</h2>
            <div class="grid grid-cols-2 border border-gray-100 max-md:grid-cols-1 my-20">
                <div v-for="(item , index) in articles" :key="index" class="flex flex-wrap gap-10 items-center p-5  border border-gray-500">
                    <img :src="item.image" alt="image...">
                    <div class="flex flex-col gap-5">
                        <h3 class="text-3xl font-semibold">{{ item.title }}</h3>
                        <div class="flex gap-8 justify-start items-center text-sm">
                            <div>
                                <span class="font-semibold pr-2">Date</span><span>16. March 2022</span>
                            </div>
                            <div>
                                <span class="font-semibold pr-2">Read</span><span>10 Min</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
