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
                <li :class="{ 'border-b-2 border-indigo-700 w-fit': $route.path === '/' }" class="mb-4">
                    <router-link to="/" class="text-base font-semibold">Home</router-link>
                </li>
                <li :class="{ 'border-b-2 border-indigo-700 w-fit': $route.path.startsWith('/category') }"
                    class="mb-4 text-base font-semibold">
                    Category
                </li>
                <li :class="{ 'border-b-2 border-indigo-700 w-fit': $route.path === '/service' }"
                    class="mb-4 text-base font-semibold">
                    Service
                </li>
                <li :class="{ 'border-b-2 border-indigo-700 w-fit': $route.path === '/about' }"
                    class="mb-4 text-base font-semibold">
                    About us
                </li>
            </ul>
        </aside>
        <!-- Header -->
        <header
            class="w-full h-auto bg-transparent-600 flex flex-row justify-between items-center p-5 pl-4 md:p-10 lg:p-16 lg:pt-15">
            <nav class="w-1/3 flex-row items-center p-4 hidden lg:flex" :class="{ 'translate-x-0': showSidebar }">
                <ul class="w-full flex flex-row justify-between">
                    <li :class="{ 'border-b-2 border-indigo-700 w-fit': $route.path === '/' }">
                        <router-link to="/" class="text-base text-gray-900 font-semibold ">Home</router-link>
                    </li>
                    <div class="relative inline-block text-left">
                        <div>
                            <button type="button" @click="toggleDropdown"
                                class="inline-flex w-full justify-center gap-x-1.5 rounded-md px-3"
                                :aria-expanded="isDropdownOpen.toString()" aria-haspopup="true">
                                <span class="text-base font-semibold text-gray-900">{{ selectedOption }}</span>
                                <svg class="-mr-1 h-5 w-5 text-gray-900" viewBox="0 0 20 20" fill="currentColor"
                                    aria-hidden="true">
                                    <path fill-rule="evenodd"
                                        d="M5.23 7.21a.75.75 0 011.06.02L10 11.168l3.71-3.938a.75.75 0 111.08 1.04l-4.25 4.5a.75.75 0 01-1.08 0l-4.25-4.5a.75.75 0 01.02-1.06z"
                                        clip-rule="evenodd" />
                                </svg>
                            </button>
                        </div>
                        <div v-show="isDropdownOpen"
                            class="absolute right-0 z-10 mt-2 w-56 origin-top-right rounded-md bg-white shadow-lg ring-1 ring-black ring-opacity-5 focus:outline-none"
                            role="menu" aria-orientation="vertical" aria-labelledby="menu-button" tabindex="-1">
                            <div class="py-1" role="none">
                                <a href="#" @click="selectOption('Main course')"
                                    class="text-gray-700 block px-4 py-2 text-sm" role="menuitem" tabindex="-1">
                                    Main course
                                </a>
                                <a href="#" @click="selectOption('Dessert')" class="text-gray-700 block px-4 py-2 text-sm"
                                    role="menuitem" tabindex="-1">
                                    Dessert
                                </a>
                                <a href="#" @click="selectOption('Salad')" class="text-gray-700 block px-4 py-2 text-sm"
                                    role="menuitem" tabindex="-1">
                                    Salad
                                </a>
                                <a href="#" @click="selectOption('Breakfast')" class="text-gray-700 block px-4 py-2 text-sm"
                                    role="menuitem" tabindex="-1">
                                    Breakfast
                                </a>
                                <a href="#" @click="selectOption('Vegetarian')" class="text-gray-700 block px-4 py-2 text-sm"
                                    role="menuitem" tabindex="-1">
                                    Vegetarian
                                </a>
                                <a href="#" @click="selectOption('Vegan')" class="text-gray-700 block px-4 py-2 text-sm"
                                    role="menuitem" tabindex="-1">
                                    Vegan
                                </a>
                                <!-- <form method="POST" action="#" role="none">
                                    <button type="submit" @click="selectOption('Sign out')"
                                        class="text-gray-700 block w-full px-4 py-2 text-left text-sm" role="menuitem"
                                        tabindex="-1">
                                        Sign out
                                    </button>
                                </form> -->
                            </div>
                        </div>
                    </div>
                    <li :class="{ 'border-b-2 border-indigo-700 w-fit': $route.path === '/service' }"
                        class="text-base text-gray-900 font-semibold">
                        Service
                    </li>
                    <li :class="{ 'border-b-2 border-indigo-700 w-fit': $route.path === '/about' }"
                        class="text-base text-gray-900 font-semibold">
                        About us
                    </li>
                </ul>
            </nav>
            <div class="flex">
                <button @click="showSidebar = !showSidebar" class="w-8 h-8 flex items-center justify-center mr-2 lg:hidden">
                    <img src="@/assets/icon/menu-icon.svg" alt="">
                </button>
                <div class="flex items-center justify-center w-[60%] md:hidden lg:flex lg:w-full">
                    <img src="@/assets/icon/resto-logo.svg" alt="">
                </div>
            </div>
            <div class="hidden items-center justify-center w-[60%] md:flex lg:hidden">
                <img src="@/assets/icon/resto-logo.svg" alt="">
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
const isDropdownOpen = ref(false);
const selectedOption = ref('Category');

const closeSidebar = () => {
    showSidebar.value = false
}

const toggleDropdown = () => {
  isDropdownOpen.value = !isDropdownOpen.value;
};

const selectOption = (option) => {
  selectedOption.value = option;
  isDropdownOpen.value = false;
};
</script>
  