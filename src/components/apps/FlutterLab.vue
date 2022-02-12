<template>
    <Window :window="this.meta">
        <template slot="content">
            <iframe src="https://flutlab.io/editor/" class="border-0 w-full h-full"></iframe>
        </template>
    </Window>
</template>

<script>
    import Window from "../window/Window";
    export default {
        name: "FlutterLab",
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
