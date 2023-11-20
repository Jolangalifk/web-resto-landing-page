<template>
    <div>
        <!-- Sidebar -->
        <aside v-if="showSidebar" class="fixed top-0 left-0 h-full w-64 bg-orange-300 text-black p-6 z-50">
            <!-- Tombol Close -->
            <button @click="closeSidebar" class="absolute top-4 right-4 text-gray-700 hover:text-gray-900">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"
                    xmlns="http://www.w3.org/2000/svg">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                </svg>
            </button>

            <!-- Konten Sidebar -->
            <ul>
                <li class="mb-2 text-base font-semibold">Home</li>
                <li class="mb-2 text-base font-semibold">Category</li>
                <li class="mb-2 text-base font-semibold">Service</li>
                <li class="mb-2 text-base font-semibold">About us</li>
            </ul>
        </aside>

        <!-- Header -->
        <header
            class="w-full h-auto bg-transparent-600 flex flex-row justify-between items-center p-5 pl-4 md:p-10 lg:p-16 lg:pt-15">
            <nav class="w-1/3 flex-row items-center p-4 hidden lg:flex" :class="{ 'translate-x-0': showSidebar }">
                <ul class="w-full flex flex-row justify-between">
                    <li class="text-base text-gray-900 font-semibold border-b-2 border-indigo-700">Home</li>
                    <div class="dropdown">
                        <button class="flex flex-row items-center">
                            <p class="text-base text-gray-900 font-semibold mr-2">Category</p>
                            <img src="@/assets/icon/arrow-down-light.svg" class="w-2 h-2" alt="">
                        </button>
                    </div>
                    <li class="text-base text-gray-900 font-semibold">Service</li>
                    <li class="text-base text-gray-900 font-semibold">About us</li>
                </ul>
            </nav>
            <div class="flex">
                <button @click="showSidebar = !showSidebar" class="w-8 h-8 flex items-center justify-center mr-2 lg:hidden">
                    <img src="@/assets/icon/menu-icon.svg" alt="">
                </button>
                <div class="flex items-center justify-center w-[60%] lg:w-full">
                    <img src="@/assets/icon/resto-logo.svg" alt="">
                </div>
            </div>
            <div class="w-24 h-full flex flex-row justify-between lg:w-1/3">
                <div class="w-3/4 hidden flex-row bg-white p-4 rounded-lg lg:flex">
                    <button class="mr-4">
                        <img src="@/assets/icon/search-icon.svg" alt="">
                    </button>
                    <input class="w-full font-medium text-black outline-0" type="text"
                        placeholder="Search your favorite food">
                </div>
                <div class="flex w-full h-10 lg:w-24 lg:h-14">
                    <button class="w-full bg-gray-200 rounded-lg">
                        <p class="text-indigo-700 font-semibold">Log in</p>
                    </button>
                </div>
            </div>
        </header>
    </div>
</template>
  
<script setup>
import { ref } from 'vue'

const showSidebar = ref(false)

const closeSidebar = () => {
  showSidebar.value = false
}
</script>