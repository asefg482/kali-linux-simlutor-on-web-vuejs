<template>
  <Window :window="this.meta">
    <template slot="content">

      <div class="w-full h-full bg-ub-grey relative text-white select-none overflow-hidden flex window-main-screen">
        <iframe src="https://www.asefg.ir/" width="100%" height="100%"></iframe>
        <div class="w-3/4 md:w-4/5 bg-ub-cool-grey h-full flex flex-col justify-start items-center">
          <div class="flex flex-col justify-start items-center">
            <br>
            <div class="w-20 md:w-28 mt-8 mx-auto bg-white rounded-full">
              <img class="w-full rounded" :src="this.images.headerIcon" alt="obj9527's Logo"/>
            </div>
            <div class="mt-4 text-lg md:text-2xl text-center px-1">
              <div>Hello <span class="font-bold">There</span></div>
              <div class="font-normal ml-1">This Web Site Created By <span class="text-pink-600 font-bold">Asef Ghorbani</span>
              </div>
            </div>
            <div class=" font-medium relative text-2xl mt-2 md:mt-4 mb-4">
              How it is made
            </div>
            <div class="w-full md:w-10/12 flex mt-4">
              <div class=" text-sm text-center md:text-base w-1/0 font-bold">Technologies used</div>
            </div>
            <div class="w-full md:w-10/12 flex justify-center items-start font-bold text-center">
              <div class="px-2 w-1/2">
                <div class="flex flex-wrap justify-center items-start w-full mt-2">
                  <img class="m-1"
                       src="https://img.shields.io/badge/-JavaScript-%23F7DF1C?style=flat&logo=javascript&logoColor=000000&labelColor=%23F7DF1C&color=%23FFCE5A"
                       alt="obj9527 javascript"/>
                  <img class="m-1" src="https://img.shields.io/badge/C-00599C?style=flat&logo=c&logoColor=white"
                       alt="obj9527 c++"/>
                  <img class="m-1" src="https://img.shields.io/badge/Java-0175C2?style=flat&logo=java&logoColor=white"
                       alt="obj9527 Java"/>
                  <img class="m-1" src="https://img.shields.io/badge/Mysql-0175C2?style=flat&logo=mysql&logoColor=white"
                       alt="obj9527 dart"/>
                  <img title="yes it's a language!" class="m-1"
                       src="https://img.shields.io/badge/-HTML5-%23E44D27?style=flat&logo=html5&logoColor=ffffff"
                       alt="obj9527 HTML"/>
                  <img src="https://img.shields.io/badge/-Sass-%23CC6699?style=flat&logo=sass&logoColor=ffffff"
                       alt="obj9527 SASS" class="m-1"/>
                  <img src="https://img.shields.io/badge/-Git-%23F05032?style=flat&logo=git&logoColor=%23ffffff"
                       alt="obj9527 git" class="m-1"/>
                  <img src="https://img.shields.io/badge/-CSS3-FFCA28?style=flat&logo=css3&logoColor=ffffff"
                       alt="obj9527 firebase" class="m-1"/>
                  <img class="m-1" src="https://img.shields.io/badge/Vue-02569B?style=flat&logo=vue&logoColor=white"
                       alt="obj9527 vue"/>
                  <img src="https://img.shields.io/badge/jQuery-0769AD?style=flat&logo=jquery&logoColor=white"
                       alt="obj9527 jquery" class="m-1"/>
                  <img class=" inline ml-1"
                       src="http://img.shields.io/badge/-Linux-0078D6?style=plastic&logo=linux&logoColor=ffffff"
                       alt="obj9527 linux"/>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </template>
  </Window>
</template>

<script>
import Window from "../window/Window";

export default {
  name: "AboutObj9527",
  props: {
    meta: {
      type: Object,
      required: true,
    }
  },
  data() {
    return {
      focusedItem: 'about',
      images: {
        headerIcon: './images/logos/wow_cat.jpg',
      },
      items: [
        {
          id: 'skills',
          title: 'About App',
          image: "./themes/Yaru/status/skills.svg",
        }
      ],
    }
  },
  components: {Window},
  methods: {
    changeFocused(id) {
      this.focusedItem = id
      console.log(this.focusedItem)
    }
  }
}
</script>
