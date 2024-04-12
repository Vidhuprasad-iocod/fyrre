<script setup>

const latestPosts = [
    {
        id: 1,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/hope-dies-last.webp',
        title: 'Hope dies last',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        id: 2,
        date: '16. March 2022',
        type: 'art',
        image: '/assets/magazine/dont-close-your-eyes.webp',
        title: 'Don’t close your eyes',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    },
    {
        id: 3,
        date: '16. March 2022',
        type: 'Sculptures',
        image: '/assets/magazine/the-best-art-museums.webp',
        title: 'The best art museums',
        content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
        text: 'Jakob Gronberg',
        duration: '1 Min'
    }
]


</script>



<template>
    <div class="mx-20 my-10">
        <div class="flex justify-between mb-20">
            <NuxtLink to="/magazine"
                class="col-span-1 text-base font-semibold flex gap-2 items-center uppercase justify-end">
                <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 24 24">
                    <path fill="black"
                        d="M7.828 11H20v2H7.828l5.364 5.364l-1.414 1.414L4 12l7.778-7.778l1.414 1.414z" />
                </svg>
                GO BACK
            </NuxtLink>
            <h3 class="text-3xl font-semibold uppercase">magazine</h3>
        </div>
        <div class="flex justify between gap-18">
            <h2 class="flex-1 text-8xl font-semibold uppercase">Hope dies last</h2>
            <p class="flex-1 text-xl font-medium">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et
                dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis
                bibendum ut. Porttitor leo a diam.
            </p>
        </div>
        <div class="flex justify-between mt-24 mb-8">
            <div class="flex gap-10 text-sm">
                <div class="flex gap-2">
                    <div class="font-semibold">Text</div>
                    <p>Jakob Gronberg</p>
                </div>
                <div class="flex gap-2">
                    <div class="font-semibold">Date</div>
                    <p>16. March 2022</p>
                </div>
                <div class="flex gap-2">
                    <div class="font-semibold">Read</div>
                    <p>2 Min</p>
                </div>
            </div>
            <div class="text-xs uppercase border border-black rounded-3xl px-3 py-2">label</div>
        </div>
        <img class="mb-24" src="/assets/magazine/hope-dies-last.webp" alt="image...">
        <div class="py-10 mb-20 mx-56 grid grid-cols-9 gap-24">
            <div class="flex flex-col gap-10 col-span-3">
                <div class="flex gap-4">
                    <img src="/assets/authors/jakob-grønberg.webp" alt="image...">
                    <h4 class="text-3xl font-semibold">Jakob Gronberg</h4>
                </div>
                <div class="pt-10 flex flex-col gap-8 border-t border-black">
                    <div class="flex justify-between items-center">
                        <h3 class="font-semibold">Date</h3>
                        <div>16. March 2022</div>
                    </div>
                    <div class="flex justify-between items-center">
                        <h3 class="font-semibold">Read</h3>
                        <div>2 Min</div>
                    </div>
                    <div class="flex justify-between items-center">
                        <h3 class="font-semibold">Share</h3>
                        <ul class="flex gap-2">
                            <li>
                                <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em"
                                    viewBox="0 0 24 24">
                                    <path :fill="color"
                                        d="M12.001 9a3 3 0 1 0 0 6a3 3 0 0 0 0-6m0-2a5 5 0 1 1 0 10a5 5 0 0 1 0-10m6.5-.25a1.25 1.25 0 0 1-2.5 0a1.25 1.25 0 0 1 2.5 0M12.001 4c-2.474 0-2.878.007-4.029.058c-.784.037-1.31.142-1.798.332a2.886 2.886 0 0 0-1.08.703a2.89 2.89 0 0 0-.704 1.08c-.19.49-.295 1.015-.331 1.798C4.007 9.075 4 9.461 4 12c0 2.475.007 2.878.058 4.029c.037.783.142 1.31.331 1.797c.17.435.37.748.702 1.08c.337.336.65.537 1.08.703c.494.191 1.02.297 1.8.333C9.075 19.994 9.461 20 12 20c2.475 0 2.878-.007 4.029-.058c.782-.037 1.308-.142 1.797-.331a2.91 2.91 0 0 0 1.08-.703c.337-.336.538-.649.704-1.08c.19-.492.296-1.018.332-1.8c.052-1.103.058-1.49.058-4.028c0-2.474-.007-2.878-.058-4.029c-.037-.782-.143-1.31-.332-1.798a2.912 2.912 0 0 0-.703-1.08a2.884 2.884 0 0 0-1.08-.704c-.49-.19-1.016-.295-1.798-.331C14.926 4.006 14.54 4 12 4m0-2c2.717 0 3.056.01 4.123.06c1.064.05 1.79.217 2.427.465c.66.254 1.216.598 1.772 1.153a4.908 4.908 0 0 1 1.153 1.772c.247.637.415 1.363.465 2.428c.047 1.066.06 1.405.06 4.122c0 2.717-.01 3.056-.06 4.122c-.05 1.065-.218 1.79-.465 2.428a4.884 4.884 0 0 1-1.153 1.772a4.915 4.915 0 0 1-1.772 1.153c-.637.247-1.363.415-2.427.465c-1.067.047-1.406.06-4.123.06c-2.717 0-3.056-.01-4.123-.06c-1.064-.05-1.789-.218-2.427-.465a4.89 4.89 0 0 1-1.772-1.153a4.905 4.905 0 0 1-1.153-1.772c-.248-.637-.415-1.363-.465-2.428C2.012 15.056 2 14.717 2 12c0-2.717.01-3.056.06-4.122c.05-1.065.217-1.79.465-2.428a4.88 4.88 0 0 1 1.153-1.772A4.897 4.897 0 0 1 5.45 2.525c.637-.248 1.362-.415 2.427-.465C8.945 2.013 9.284 2 12.001 2" />
                                </svg>
                            </li>
                            <li>
                                <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em"
                                    viewBox="0 0 24 24">
                                    <path :fill="color" fill-rule="evenodd"
                                        d="M22 5.892a8.178 8.178 0 0 1-2.355.635a4.074 4.074 0 0 0 1.8-2.235a8.343 8.343 0 0 1-2.605.981A4.13 4.13 0 0 0 15.85 4a4.068 4.068 0 0 0-4.1 4.038c0 .31.035.618.105.919A11.705 11.705 0 0 1 3.4 4.734a4.006 4.006 0 0 0 1.268 5.392a4.165 4.165 0 0 1-1.859-.5v.05A4.057 4.057 0 0 0 6.1 13.635a4.192 4.192 0 0 1-1.856.07a4.108 4.108 0 0 0 3.831 2.807A8.36 8.36 0 0 1 2 18.184A11.732 11.732 0 0 0 8.291 20A11.502 11.502 0 0 0 19.964 8.5c0-.177 0-.349-.012-.523A8.143 8.143 0 0 0 22 5.892"
                                        clip-rule="evenodd" />
                                </svg>
                            </li>
                            <li>
                                <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em"
                                    viewBox="0 0 24 24">
                                    <path :fill="color" fill-rule="evenodd"
                                        d="M21.7 8.037a4.26 4.26 0 0 0-.789-1.964a2.84 2.84 0 0 0-1.984-.839c-2.767-.2-6.926-.2-6.926-.2s-4.157 0-6.928.2a2.836 2.836 0 0 0-1.983.839a4.225 4.225 0 0 0-.79 1.965a30.146 30.146 0 0 0-.2 3.206v1.5a30.12 30.12 0 0 0 .2 3.206c.094.712.364 1.39.784 1.972c.604.536 1.38.837 2.187.848c1.583.151 6.731.2 6.731.2s4.161 0 6.928-.2a2.844 2.844 0 0 0 1.985-.84a4.27 4.27 0 0 0 .787-1.965a30.12 30.12 0 0 0 .2-3.206v-1.516a30.672 30.672 0 0 0-.202-3.206m-11.692 6.554v-5.62l5.4 2.819z"
                                        clip-rule="evenodd" />
                                </svg>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="flex flex-col gap-10 col-span-6">
                <p class="text-xl font-medium">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
                    tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem.
                    Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.
                </p>
                <p class="whitespace-pre-line">
                    Porttitor rhoncus dolor purus non enim praesent elementum. Eget dolor morbi non arcu risus quis
                    varius. Posuere ac ut consequat semper viverra nam libero. In ornare quam viverra orci sagittis eu.
                    Tristique risus nec feugiat in fermentum posuere urna nec. Tempus quam pellentesque nec nam aliquam
                    sem et. Convallis a cras semper auctor neque vitae tempus quam pellentesque. Sollicitudin ac orci
                    phasellus egestas tellus rutrum tellus pellentesque. Sed egestas egestas fringilla phasellus
                    faucibus scelerisque eleifend donec pretium. Sit amet porttitor eget dolor morbi non arcu risus.
                    Justo eget magna fermentum iaculis eu non diam phasellus. Sit amet luctus venenatis lectus magna
                    fringilla. Neque vitae tempus quam pellentesque nec nam. {{ '\n' }}{{ '\n' }}

                    Tellus orci ac auctor augue mauris augue neque gravida. Tempus imperdiet nulla malesuada
                    pellentesque elit eget gravida cum sociis. Id eu nisl nunc mi ipsum faucibus vitae aliquet. Duis
                    convallis convallis tellus id interdum velit laoreet id. Vulputate mi sit amet mauris commodo quis.
                    Semper viverra nam libero justo laoreet sit amet. Eget nullam non nisi est sit. Nibh cras pulvinar
                    mattis nunc sed blandit libero. Ac felis donec et odio pellentesque diam volutpat. Quis varius quam
                    quisque id diam vel quam elementum. Felis bibendum ut tristique et egestas quis ipsum suspendisse
                    ultrices. Id diam vel quam elementum pulvinar etiam non. Non consectetur a erat nam at lectus urna
                    duis convallis.
                </p>
                <div class="flex gap-5 py-10 border-y border-black">
                    <h1 class="font-semibold text-8xl">“</h1>
                    <div>
                        <h1 class="text-5xl font-semibold leading-1">
                            The greatest glory in living lies not in never
                            falling, but in rising every time we fall.
                        </h1>
                        <h6 class="text-sm mt-6">Nelson Mandela</h6>
                    </div>
                </div>
                <p class="text-xl font-medium">
                    Est pellentesque elit ullamcorper dignissim. Consectetur a erat nam at. Blandit libero volutpat sed
                    cras ornare arcu. Iaculis urna id volutpat lacus laoreet. Tincidunt ornare massa eget egestas purus
                    viverra accumsan in. Viverra ipsum nunc aliquet bibendum enim facilisis gravida neque.
                </p>
                <p class="whitespace-pre-line">
                    Vitae turpis massa sed elementum tempus egestas sed. Quam lacus suspendisse faucibus interdum
                    posuere lorem ipsum. Viverra justo nec ultrices dui sapien eget. At risus viverra adipiscing at in
                    tellus integer feugiat. Elementum eu facilisis sed odio morbi quis commodo. Arcu cursus vitae congue
                    mauris rhoncus aenean. Auctor elit sed vulputate mi sit amet mauris commodo quis. Lectus sit amet
                    est placerat in egestas erat imperdiet sed. Eu mi bibendum neque egestas congue quisque. Sit amet
                    luctus venenatis lectus magna fringilla urna porttitor. Pretium vulputate sapien nec sagittis
                    aliquam malesuada bibendum arcu. Sed ullamcorper morbi tincidunt ornare massa eget egestas purus.
                    Pharetra vel turpis nunc eget lorem. Morbi blandit cursus risus at ultrices mi tempus imperdiet
                    nulla. In metus vulputate eu scelerisque felis imperdiet. Elementum pulvinar etiam non quam lacus
                    suspendisse. Sem fringilla ut morbi tincidunt augue. Id venenatis a condimentum vitae sapien. Varius
                    quam quisque id diam vel. {{ '\n' }}{{ '\n' }}

                    Nec feugiat in fermentum posuere urna nec tincidunt praesent semper. Aliquam nulla facilisi cras
                    fermentum. Quam elementum pulvinar etiam non quam lacus suspendisse faucibus interdum. Neque vitae
                    tempus quam pellentesque nec. Interdum consectetur libero id faucibus nisl tincidunt eget nullam.
                    Mattis enim ut tellus elementum sagittis. In fermentum et sollicitudin ac orci phasellus. Est sit
                    amet facilisis magna etiam tempor orci. Lacinia at quis risus sed vulputate odio ut. Egestas egestas
                    fringilla phasellus faucibus scelerisque eleifend. Nunc pulvinar sapien et ligula ullamcorper
                    malesuada proin libero. Aenean vel elit scelerisque mauris pellentesque. Gravida arcu ac tortor
                    dignissim. Ac tortor dignissim convallis aenean.
                </p>
            </div>
        </div>
        <div class="mb-20 pb-20">
            <div class="flex justify-between items-center border-t border-black pt-10 mb-24">
                <h1 class="font-semibold text-8xl uppercase">Latest posts</h1>
                <NuxtLink class="uppercase font-semibold flex items-center gap-2" to="/magazine">
                    see all
                    <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 24 24">
                        <path fill="black"
                            d="m16.172 11l-5.364-5.364l1.414-1.414L20 12l-7.778 7.778l-1.414-1.414L16.172 13H4v-2z" />
                    </svg>
                </NuxtLink>
            </div>
            <div class="grid grid-cols-3">
                <div v-for="(item, index) in latestPosts" :key="index" class="p-10 flex flex-col gap-5 border border-black">
                    <div class="flex justify-between">
                        <p class="text-sm">{{ item.date }}</p>
                        <label class="text-xs uppercase border border-black rounded-3xl px-3 py-2" for="">{{ item.type}}</label>
                    </div>
                    <NuxtLink to="/magazine/magazinePost">
                        <img :src="item.image" alt="image...">
                    </NuxtLink>
                    <div class="flex gap-20 flex-col justify-between">
                        <div class="flex flex-col gap-2">
                            <h2 class="text-3xl font-semibold">{{ item.title }}</h2>
                            <p class="text-justify">{{ item.content }}</p>
                        </div>
                        <div>
                            <div class="flex justify-between">
                                <div class="flex gap-8 justify-start items-center text-sm">
                                    <div>
                                        <span class="font-semibold pr-2">Text</span><span>{{ item.text }}</span>
                                    </div>
                                    <div>
                                        <span class="font-semibold pr-2">Duration</span><span>{{ item.duration }}</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>