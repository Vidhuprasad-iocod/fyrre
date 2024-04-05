
<template>
    <header class="mx-20 mt-6">
        <div class=" flex flex-wrap justify-between items-center">
            <NuxtLink to="/">
                <img src="/assets/header/fyrreMagazine.svg" alt="image...">
            </NuxtLink>
            <ul class="flex flex-wrap gap-5 items-center">
                <li><nuxt-link to="/magazine">Magazine</nuxt-link></li>
                <li><nuxt-link to="/authors">Authors</nuxt-link></li>
                <li><nuxt-link to="/podcasts">Podcast</nuxt-link></li>
                <li class="border border-black w-4"></li>
                <li>
                    <social-media color="black"/>
                </li>
            </ul>
        </div>
        <div class="border border-black mt-4"></div>
    </header>
</template>


