<template>
    <div :style="{backgroundImage: `url(${this.bg_images[this.wallpaper]})`}"
         style="background-size: cover;background-repeat: no-repeat;background-position-x: center"
         class="bg-ubuntu-img absolute -z-10 top-0 right-0 overflow-hidden h-full w-full">
    </div>
</template>

<script>
    export default {
        name: "BackgroundImage",
        props: {
            wallpaper: {
                type: String,
            }
        },
        data() {
            return {
                bg_images: {
                    'wall-1': "./images/wallpapers/wall-1.png",
                    'wall-2': "./images/wallpapers/wall-2.jpg",
                    'wall-3': "./images/wallpapers/wall-3.jpg",
                    'wall-4': "./images/wallpapers/wall-4.jpg",
                    'wall-5': "./images/wallpapers/wall-5.png",
                    'wall-6': "./images/wallpapers/wall-6.png",
                    'wall-7': "./images/wallpapers/wall-7.jpg",
                    'wall-8': "./images/wallpapers/wall-8.jpg",
                },
            }
        },
    }
</script>
