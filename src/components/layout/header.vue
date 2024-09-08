<template>
    <header class="sticky top-0 z-[999]">
        <div class="flex flex-col bg-custom-red p-4 w-full ">
            <div class="flex justify-end ">
                <input type="search" placeholder="搜索" class="px-4 py-2  rounded-lg">
            </div>
        </div>
        <nav x-data="{ open: false }"  class="flex h-auto w-auto bg-white shadow-lg rounded-lg justify-between
            md:h-16">
            <div class="flex w-full justify-between ">
                <div :class="open ? 'hidden':'flex'" 
                class="flex px-6 w-1/2 items-center font-semibold
                md:w-1/5 md:px-1 md:flex md:items-center md:justify-center"
                x-transition:enter="transition ease-out duration-300">
                    <div class="logo">
                        <img src="/logo.png" alt="Logo">
                    </div>
                </div>

                <div class="hidden w-3/5 items-center justify-evenly font-semibold
                md:flex">
                    <a href="">首页</a>
                    <a href="">关于</a>
                    <a href="">产品</a>
                    <a href="">博客</a>
                    <a href="">职业</a>
                    <a href="">联络</a>
                </div>

                <button class="text-gray-500 w-10 h-10 relative focus:outline-none bg-white
                                md:hidden
                                " @click="open = !open">
                    <span class="sr-only">Open main menu</span>
                    <div class="block w-5 absolute left-1/2 top-1/2   transform  -translate-x-1/2 -translate-y-1/2">
                        <span aria-hidden="true" class="block absolute h-0.5 w-5 bg-current transform transition duration-500 ease-in-out" :class="{'rotate-45': open,' -translate-y-1.5': !open }"></span>
                        <span aria-hidden="true" class="block absolute  h-0.5 w-5 bg-current   transform transition duration-500 ease-in-out" :class="{'opacity-0': open } "></span>
                        <span aria-hidden="true" class="block absolute  h-0.5 w-5 bg-current transform  transition duration-500 ease-in-out" :class="{'-rotate-45': open, ' translate-y-1.5': !open}"></span>
                    </div>
                </button>
            </div>
        </nav>
    </header>
</template>
  
  
  <script setup>
  import { ref } from 'vue'
  
  const menuOpen = ref(false)
  
  const toggleMenu = () => {
    menuOpen.value = !menuOpen.value
  }

  
  </script>
  
  <style scoped>
  /* You can add any additional custom styles here */
  .bg-custom-red {
    background-color: #B3272D;
  }
  </style>