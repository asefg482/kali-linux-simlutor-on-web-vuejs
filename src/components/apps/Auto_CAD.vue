<template>
    <Window :window="this.meta">
        <template slot="content">
            <iframe src="https://web.autocad.com/login" class="border-0 w-full h-full"></iframe>
<!--            <iframe src="https://www.google.com/" class="border-0 w-full h-full"></iframe>-->
        </template>
    </Window>
</template>

<script>
    import Window from "../window/Window";
    export default {
        name: "Auto_CAD",
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
