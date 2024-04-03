<template>
    <ul class="flex gap-2 items-center">
        <li>
            <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 24 24">
	            <g fill="none" :stroke="color" stroke-width="1.5">
	            	<path stroke-linecap="round" stroke-linejoin="round" d="M12 16a4 4 0 1 0 0-8a4 4 0 0 0 0 8" />
	            	<path d="M3 16V8a5 5 0 0 1 5-5h8a5 5 0 0 1 5 5v8a5 5 0 0 1-5 5H8a5 5 0 0 1-5-5Z" />
	            	<path stroke-linecap="round" stroke-linejoin="round" d="m17.5 6.51l.01-.011" />
	            </g>
	        </svg>
        </li>
        <li>
            <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 24 24">
	            <path :fill="color" fill-rule="evenodd" d="M22 5.892a8.178 8.178 0 0 1-2.355.635a4.074 4.074 0 0 0 1.8-2.235a8.343 8.343 0 0 1-2.605.981A4.13 4.13 0 0 0 15.85 4a4.068 4.068 0 0 0-4.1 4.038c0 .31.035.618.105.919A11.705 11.705 0 0 1 3.4 4.734a4.006 4.006 0 0 0 1.268 5.392a4.165 4.165 0 0 1-1.859-.5v.05A4.057 4.057 0 0 0 6.1 13.635a4.192 4.192 0 0 1-1.856.07a4.108 4.108 0 0 0 3.831 2.807A8.36 8.36 0 0 1 2 18.184A11.732 11.732 0 0 0 8.291 20A11.502 11.502 0 0 0 19.964 8.5c0-.177 0-.349-.012-.523A8.143 8.143 0 0 0 22 5.892" clip-rule="evenodd" />
	        </svg>
        </li>
        <li>
            <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 24 24">
	            <path :fill="color" fill-rule="evenodd" d="M21.7 8.037a4.26 4.26 0 0 0-.789-1.964a2.84 2.84 0 0 0-1.984-.839c-2.767-.2-6.926-.2-6.926-.2s-4.157 0-6.928.2a2.836 2.836 0 0 0-1.983.839a4.225 4.225 0 0 0-.79 1.965a30.146 30.146 0 0 0-.2 3.206v1.5a30.12 30.12 0 0 0 .2 3.206c.094.712.364 1.39.784 1.972c.604.536 1.38.837 2.187.848c1.583.151 6.731.2 6.731.2s4.161 0 6.928-.2a2.844 2.844 0 0 0 1.985-.84a4.27 4.27 0 0 0 .787-1.965a30.12 30.12 0 0 0 .2-3.206v-1.516a30.672 30.672 0 0 0-.202-3.206m-11.692 6.554v-5.62l5.4 2.819z" clip-rule="evenodd" />
	        </svg>
        </li>
        <li>
            <svg xmlns="http://www.w3.org/2000/svg" width="1.5em" height="1.5em" viewBox="0 0 256 256">
	            <path :fill="color" d="M220 200a12 12 0 0 1-24 0c0-77.2-62.8-140-140-140a12 12 0 0 1 0-24c90.43 0 164 73.57 164 164M56 108a12 12 0 0 0 0 24a68.07 68.07 0 0 1 68 68a12 12 0 0 0 24 0a92.1 92.1 0 0 0-92-92m4 72a16 16 0 1 0 16 16a16 16 0 0 0-16-16" />
	        </svg>
        </li>
    </ul>
</template>



<script setup>

defineProps({
    color: String,
    default: "black"
})

defineComponent({
  name: ['IconoirInstagram','FlowbiteTwitterSolid','FlowbiteYoutubeSolid','PhRssSimpleBold']
});
</script>

	
