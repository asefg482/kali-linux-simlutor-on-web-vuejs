<template>
    <div class="relative duration-500 select-none flex flex-col justify-around items-center top-0 right-0 overflow-hidden m-0 p-0 h-screen w-screen bg-ub-violet" style="background-color: #00040a">
        <img class="md:w-1/4 w-1/2" :src="this.icons.Page_Main" alt="Ubuntu Logo"/>
        <div class="w-10 h-10 flex justify-center items-center rounded-full outline-none cursor-pointer" @click="turnOn">
            <div class="rounded-full flex justify-center items-center w-10 h-10 hover:bg-gray-300" :class="this.isBoot ? 'hover:bg-ub-violet':'bg-white'">
                <img v-if="!isBoot" class="w-8" :src="this.icons.powerButton" alt="Power Button">
            </div>
        </div>
        <p style="font-size: 50px;font-family: Roboto;color: white">Online Kali Linux</p>
        <div class="text-white mb-4">
            <a class="underline" href="https://asefg.ir" rel=""
               target="_blank">My Web Site</a>
            <span class="font-bold mx-1">|</span>
            <a href="My Instagram" rel="" target="_blank"
               class="underline">Instagram</a>
        </div>
    </div>
</template>
<script>
    export default {
        name: 'Login',
        data() {
            return {
                icons: {
                    Page_Main: './images/wallpapers/wall-1.png',
                    powerButton: './themes/Yaru/status/power-button.svg',
                    processSymbol: './themes/Yaru/status/process-working-symbolic.svg',
                  Kali_Type:'./themes/Yaru/status/Kali_Type.jpg'
                },
                isBoot: false,
            }
        },
        methods: {
            turnOn() {
                this.isBoot = true
                setTimeout(() => {
                    this.fullScreen()
                    this.$router.push('/desktop')
                }, 2000)
            },
            fullScreen() {
                let element = document.documentElement;
                if (element.requestFullscreen) {
                    element.requestFullscreen()
                } else if (element.msRequestFullscreen) {
                    element.msRequestFullscreen()
                } else if (element.mozRequestFullScreen) {
                    element.mozRequestFullScreen()
                } else if (element.webkitRequestFullscreen) {
                    element.webkitRequestFullscreen()
                }
            }
        }
    }
</script>
