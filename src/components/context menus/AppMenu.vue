<template>
    <div id="app-menu" class="w-52 bg-ub-context-menu border text-left border-gray-900 rounded text-white py-4 absolute z-50 text-sm flex flex-col items-start"
            :class="this.$store.state.showAppMenu ? 'block':'hidden'">
        <a rel="noreferrer noopener" href="Data :)" target="_blank" class="w-full block cursor-default py-0.5 hover:bg-ub-warm-grey hover:bg-opacity-20 mb-1.5">
            <span class="ml-5">🌟</span> <span class="ml-2">Get Data</span>
        </a>
        <Separator class="w-52"/>
        <a rel="noreferrer noopener" href="Report Bug" target="_blank" class="w-full block cursor-default py-0.5 hover:bg-ub-warm-grey hover:bg-opacity-20 mb-1.5">
            <span class="ml-7">❗</span> <span class="ml-3">Report bugs</span>
        </a>
        <a rel="noreferrer noopener" href="https://www.asefg.ir/" target="_blank" class="w-full block cursor-default py-0.5 hover:bg-ub-warm-grey hover:bg-opacity-20 mb-1.5">
            <span class="ml-5">🙋‍♂️</span> <span class="ml-2">Me Web <strong>Site</strong></span>
        </a>
        <a rel="noreferrer noopener" href="https://www.instagram.com/asef_9082/" target="_blank" class="w-full block cursor-default py-0.5 hover:bg-ub-warm-grey hover:bg-opacity-20 mb-1.5">
            <span class="ml-5">🤝</span> <span class="ml-2">Follow on <strong>instagram</strong></span>
        </a>
        <Separator class="w-52"/>
        <a rel="noreferrer noopener" href="Source Code :|" target="_blank" class="w-full block cursor-default py-0.5 hover:bg-ub-warm-grey hover:bg-opacity-20 mb-1.5">
            <span class="ml-5">📥</span> <span class="ml-2">Download Source Code :)</span>
        </a>
    </div>
</template>

<script>
    import Separator from "@/components/utils/Separator";
    export default {
        name: "AppMenu",
        components: {Separator}
    }
</script>
