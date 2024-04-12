<script setup>
import gsap from 'gsap'

onMounted( () => {
    gsap.to('#titleName', {
        opacity: 1,
        y: 0,
        duration: 1,
        ease: 'power2.out'
    })
})

</script>


<template>
    <div class="mx-20 my-10 flex flex-col gap-20">
        <img id="titleName" class="relative opacity-0 translate-y-40" src="/assets/magazine/Magazine.svg" alt="image...">
        <div class="flex justify-between items-center">
            <h6 class="uppercase font-semibold">Categories</h6>
            <div class="flex gap-2 text-xs">
                <label class="uppercase border border-black rounded-3xl px-3 py-2" for="">all</label>
                <label class="uppercase border border-black rounded-3xl px-3 py-2" for="">art</label>
                <label class="uppercase border border-black rounded-3xl px-3 py-2" for="">street art</label>
                <label class="uppercase border border-black rounded-3xl px-3 py-2" for="">Sculptures</label>
            </div>
        </div>
        <MagazineMagazines />
       <div class="flex justify-end mb-20">
            <a class="font-semibold flex gap-2 items-center uppercase" href="">next
                <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24">
		            <path fill="black" d="m16.172 11l-5.364-5.364l1.414-1.414L20 12l-7.778 7.778l-1.414-1.414L16.172 13H4v-2z" />
	            </svg>
            </a>
       </div>
    </div>
</template>