<template>
    <Window :window="this.meta">
        <template slot="content">
            <iframe src="https://codesandbox.io/s/" class="border-0 w-full h-full"></iframe>
        </template>
    </Window>
</template>

<script>
    import Window from "../window/Window";
    export default {
        name: "Autocad",
        components: {Window},
        props: {
            meta: {
                type: Object,
                required: true,
            }
        }
    }
</script>

<style scoped>

</style>
