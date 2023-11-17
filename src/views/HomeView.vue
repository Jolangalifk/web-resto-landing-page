<script setup>
import TheWelcome from '../components/TheWelcome.vue'
import Navbar from '../components/Navbar.vue'
</script>

<template>
  <main class=" bg-gray-100">
    <Navbar />
    <body>
      <div class="items-center w-full p-5 mb-36 md:mb-10 lg:justify-end lg:px-16 lg:mb-14 flex">
        <div class="absolute right-[14%] top-[30%] md:right-[30%] md:left-[30%] md:top-[30%] lg:top-[45%] lg:absolute lg:left-12">
          <div class="w-[280px] h-[175px] p-4 lg:w-[430px] lg:h-[300px] bg-white rounded-3xl lg:p-6 flex flex-col">
            <div class="flex items-center mb-1">
              <svg class="w-3 h-3 lg:w-4 lg:h-4 ms-1 text-yellow-500" aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 22 20">
                <path
                  d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
              </svg>
              <svg class="w-3 h-3 lg:w-4 lg:h-4 ms-1 text-yellow-500" aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 22 20">
                <path
                  d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
              </svg>
              <svg class="w-3 h-3 lg:w-4 lg:h-4 ms-1 text-yellow-500" aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 22 20">
                <path
                  d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
              </svg>
              <svg class="w-3 h-3 lg:w-4 lg:h-4 ms-1 text-yellow-500" aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 22 20">
                <path
                  d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
              </svg>
              <svg class="w-3 h-3 lg:w-4 lg:h-4 ms-1 text-yellow-500 mr-2" aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 22 20">
                <path
                  d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
              </svg>
              <p class="font-semibold text-xs lg:text-lg text-yellow-500 mr-2">5.0</p>
              <p class="text-gray-700 text-xs lg:text-base">(5.2K+)</p>
            </div>
            <h1 class="font-semibold text-lg lg:text-2xl text-black mb-1">Padang Restaurant</h1>
            <p class="font-semibold text-sm text-gray-700 lg:text-lg mb-1">IDR 49.999 - IDR 560.000</p>
            <div class="flex mb-2 lg:mb-8">
              <img src="@/assets/icon/location.svg" class="w-4 h-4" alt="">
              <p class="text-gray-700 text-xs ml-1 lg:text-base lg:ml-2">Padang, Indonesia</p>
            </div>
            <button
              class="w-full h-11 lg:w-fit lg:h-14 bg-orange-300 rounded-xl p-4 flex items-center justify-center px-7 py-4 mb-3">
              <p class="font-semibold text-xs lg:text-base text-black mr-2">Make Reservation</p>
              <img src="@/assets/icon/arrow.svg" class="w-2 h-2" alt="">
            </button>
            <div class="hidden lg:flex">
              <img src="@/assets/icon/info-square.svg" alt="">
              <p class="text-gray-700 text-base ml-2">No extra cost</p>
            </div>
          </div>
        </div>
        <img src="@/assets/image/bg-resto.png" class="rounded-3xl lg:w-[91%]" alt="">
      </div>
      <div class="w-full px-5 flex flex-col mb-10 lg:px-16 lg:mb-40">
        <div class="flex flex-col items-center justify-center mb-5 lg:mb-10">
          <p class="font-semibold text-xs mb-2 lg:text-base text-indigo-700 lg:mb-4">SPECIAL BENEFIT FOR YOU</p>
          <h1 class="font-semibold text-base lg:text-3xl text-gray-900">Why Should Choose Us?</h1>
        </div>
        <div class="flex items-center flex-col lg:flex-row lg:justify-between">
          <div
            class="flex flex-col items-center justify-center mb-6 p-5 lg:p-0 md:w-full md:items-start lg:w-[335px] lg:h-[367px] rounded-3xl lg:pt-6 bg-white lg:justify-between overflow-hidden lg:mb-0">
            <div class="flex mb-6 items-center lg:justify-center lg:flex-col lg:mb-0">
              <div class="flex w-20 h-16 md:h-20 lg:h-20 rounded-full bg-orange-100 items-center justify-center lg:mb-6">
                <img src="@/assets/icon/discount.svg" class="w-[60%] lg:w-[70%]" alt="">
              </div>
              <div class="flex flex-col w-fit ml-4 lg:items-center lg:justify-center">
                <h1 class="font-semibold text-base text-gray-900 lg:text-lg mb-2 w-fit">Extra Discounts</h1>
                <p class="text-gray-700 text-xs lg:text-base lg:text-center w-[80%]">Get your special discount by using
                  our reservation
                </p>
              </div>
            </div>
            <button
              class="flex w-full h-10 lg:h-16 rounded-xl items-center justify-center bg-white hover:bg-orange-300 transition-colors duration-500 ease-in-out">
              <p class="font-semibold text-xs lg:text-base text-black mr-2">View Details</p>
              <img src="@/assets/icon/arrow.svg" class="w-2 h-2" alt="">
            </button>
          </div>
          <div
            class="flex flex-col items-center justify-center mb-6 p-5 lg:p-0 md:w-full md:items-start lg:w-[335px] lg:h-[367px] rounded-3xl lg:pt-6 bg-white lg:justify-between overflow-hidden lg:mb-0">
            <div class="flex mb-6 items-center lg:justify-center lg:flex-col lg:mb-0">
              <div class="flex w-20 h-16 md:h-20 lg:h-20 rounded-full bg-orange-100 items-center justify-center lg:mb-6">
                <img src="@/assets/icon/menu.svg" class="w-[60%] lg:w-[70%]" alt="">
              </div>
              <div class="flex flex-col w-fit ml-4 lg:items-center lg:justify-center">
                <h1 class="font-semibold text-base text-gray-900 lg:text-lg mb-2 w-fit">Come and Eat</h1>
                <p class="text-gray-700 text-xs lg:text-base lg:text-center w-[80%]">Get your own table quickly & without
                  waiting in
                  line
                </p>
              </div>
            </div>
            <button
              class="flex w-full h-10 lg:h-16 rounded-xl items-center justify-center bg-white hover:bg-orange-300 transition-colors duration-500 ease-in-out">
              <p class="font-semibold text-xs lg:text-base text-black mr-2">View Details</p>
              <img src="@/assets/icon/arrow.svg" class="w-2 h-2" alt="">
            </button>
          </div>
          <div
            class="flex flex-col items-center justify-center mb-6 p-5 lg:p-0 md:w-full md:items-start lg:w-[335px] lg:h-[367px] rounded-3xl lg:pt-6 bg-white lg:justify-between overflow-hidden lg:mb-0">
            <div class="flex mb-6 items-center lg:justify-center lg:flex-col lg:mb-0">
              <div class="flex w-20 h-16 md:h-20 lg:h-20 rounded-full bg-orange-100 items-center justify-center lg:mb-6">
                <img src="@/assets/icon/dolar.svg" class="w-[60%] lg:w-[70%]" alt="">
              </div>
              <div class="flex flex-col w-fit ml-4 lg:items-center lg:justify-center">
                <h1 class="font-semibold text-base text-gray-900 lg:text-lg mb-2 w-fit">No Extra Fee</h1>
                <p class="text-gray-700 text-xs lg:text-base lg:text-center w-[80%]">Get tax free if you want to order
                  food and make a reservation
                </p>
              </div>
            </div>
            <button
              class="flex w-full h-10 lg:h-16 rounded-xl items-center justify-center bg-white hover:bg-orange-300 transition-colors duration-500 ease-in-out">
              <p class="font-semibold text-xs lg:text-base text-black mr-2">View Details</p>
              <img src="@/assets/icon/arrow.svg" class="w-2 h-2" alt="">
            </button>
          </div>
          <div
            class="flex flex-col items-center justify-center mb-6 p-5 lg:p-0 md:w-full md:items-start lg:w-[335px] lg:h-[367px] rounded-3xl lg:pt-6 bg-white lg:justify-between overflow-hidden lg:mb-0">
            <div class="flex mb-6 items-center lg:justify-center lg:flex-col lg:mb-0">
              <div class="flex w-20 h-16 md:h-20 lg:h-20 rounded-full bg-orange-100 items-center justify-center lg:mb-6">
                <img src="@/assets/icon/cleanliness.svg" class="w-[60%] lg:w-[70%]" alt="">
              </div>
              <div class="flex flex-col w-fit ml-4 lg:items-center lg:justify-center">
                <h1 class="font-semibold text-base text-gray-900 lg:text-lg mb-2 w-fit">Guaranteed Cleanliness</h1>
                <p class="text-gray-700 text-xs lg:text-base lg:text-center w-[90%]">We ensure the cleanliness of the
                  place as well as the food
                </p>
              </div>
            </div>
            <button
              class="flex w-full h-10 lg:h-16 rounded-xl items-center justify-center bg-white hover:bg-orange-300 transition-colors duration-500 ease-in-out">
              <p class="font-semibold text-xs lg:text-base text-black mr-2">View Details</p>
              <img src="@/assets/icon/arrow.svg" class="w-2 h-2" alt="">
            </button>
          </div>
        </div>
      </div>
      <div class="flex flex-col px-16 justify-between mb-14 lg:mb-40 lg:flex-row">
        <div class="flex flex-col w-full justify-center items-center mb-8 lg:items-start lg:mb-0">
          <p class="font-semibold text-center text-xs mb-2 lg:text-base text-indigo-700 lg:mb-4 lg:text-start">TOP 3
            FEATURED RESTAURANT</p>
          <h1 class="font-semibold text-center text-base mb-4 lg:text-3xl text-gray-900 lg:mb-8 lg:text-start">Most
            Popular Restaurants</h1>
          <p class="text-gray-700 text-center text-xs mb-4 lg:text-base lg:w-[60%] lg:mb-14 lg:text-start">The best
            restaurant in our opinion is how much customers like
            it in terms of place, price, comfort and of course the taste of
            the food itself.</p>
          <button class="w-fit h-11 lg:h-14 bg-orange-300 rounded-xl p-4 flex items-center justify-center px-7 py-4">
            <p class="font-semibold text-xs lg:text-base text-black mr-2">View All Restaurant</p>
            <img src="@/assets/icon/arrow.svg" class="w-2 h-2" alt="">
          </button>
        </div>
        <div class="flex gap-x-3 lg:gap-x-6">
          <div class="rounded-3xl flex flex-col items-end w-full lg:h-[475px] lg:w-[400px] ">
            <img class="rounded-3xl h-full" src="@/assets/image/bg-1.png" alt="">
            <div
              class="flex absolute p-4 left-[24%] top-[233%] md:w-80 md:left-[12%] md:top-[268%] lg:h-32 w-fit rounded-3xl justify-between items-center lg:left-[40%] lg:w-[20%] lg:top-[238%] lg:p-6 lg:z-10 lg:m-6 bg-white">
              <div class="flex flex-col">
                <div class="flex flex-row items-center">
                  <svg class="w-4 h-4 ms-1 text-yellow-500 mr-2" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                    fill="currentColor" viewBox="0 0 22 20">
                    <path
                      d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
                  </svg>
                  <p class="font-semibold text-xs lg:text-lg text-yellow-500 mr-2">5.0</p>
                  <p class="text-gray-700 text-xs lg:text-base">(7.6K+)</p>
                </div>
                <div class="flex flex-col">
                  <h1 class="font-semibold text-base lg:text-2xl text-black mb-1">Bind Balorant</h1>
                  <div class="flex">
                    <img src="@/assets/icon/location.svg" class="w-4 h-4" alt="">
                    <p class="text-gray-700 text-xs lg:text-base ml-1 lg:ml-2">Padang, Indonesia</p>
                  </div>
                </div>
              </div>
              <button
                class="flex items-center justify-center w-6 h-6 ml-4 rounded-lg lg:w-9 lg:h-9 lg:ml-6 lg:rounded-xl bg-orange-300">
                <img src="@/assets/icon/arrow-right-1.svg" alt="">
              </button>
            </div>
          </div>
          <div class="rounded-3xl hidden md:flex lg:w-[214px] lg:h-[475px] lg:flex">
            <img class="rounded-3xl object-cover" src="@/assets/image/bg-2.png" alt="">
          </div>
          <div class="rounded-3xl hidden md:flex lg:w-[214px] lg:h-[475px] lg:flex">
            <img class="rounded-3xl object-cover" src="@/assets/image/bg-3.png" alt="">
          </div>
        </div>
      </div>
      <div class="w-full px-16 mb-14 lg:mb-40">
        <div class="flex flex-col w-full justify-between items-center mb-8 md:flex-row lg:items-start lg:flex-row lg:mb-0">
          <div class="flex flex-col mb-4 lg:mb-8">
            <p class="font-semibold text-xs mb-2 lg:text-base text-indigo-700 lg:mb-3">RESTAURANT BASED BY CITY</p>
            <h1 class="font-semibold text-base lg:text-3xl text-gray-900">Restaurant Near You</h1>
          </div>
          <div class="flex w-48 h-11 p-2 lg:w-64 lg:h-16 rounded-xl bg-gray-200 justify-between items-center lg:p-6">
            <img src="@/assets/icon/location.svg" class="w-4 h-4 lg:w-6 lg:h-6" alt="">
            <p class="font-medium text-xs lg:text-base text-gray-600">Jakarta, Indonesia</p>
            <button>
              <img src="@/assets/icon/arrow-down-light.svg" class="w-3 h-3 lg:w-2 lg:h-2" alt="">
            </button>
          </div>
        </div>
        <div class="flex flex-col justify-between mb-8 md:items-center lg:mb-14 lg:flex-row">
          <div class="rounded-3xl flex items-end mb-4 md:w-[60%] lg:mb-0 lg:h-[415px] lg:w-[427px] ">
            <img class="rounded-3xl w-full lg:w-auto lg:absolute" src="@/assets/image/resto-1.png" alt="">
            <div
              class="absolute flex lg:w-fit lg:h-32 w-fit rounded-3xl justify-between items-center ml-3 mb-3 p-4 md:w-[47%] lg:p-6 z-10 lg:m-6 bg-white lg:flex">
              <div class="flex flex-col mr-6 lg:mr-[75px]">
                <div class="flex flex-row items-center">
                  <svg class="w-4 h-4 ms-1 text-yellow-500 mr-2" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                    fill="currentColor" viewBox="0 0 22 20">
                    <path
                      d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
                  </svg>
                  <p class="font-semibold text-xs lg:text-lg text-yellow-500 mr-2">5.0</p>
                  <p class="text-gray-700 text-xs lg:text-base">(6.6K+)</p>
                </div>
                <h1 class="font-semibold text-base text-black mb-1">Batavia Restaurant</h1>
                <p class="text-gray-700 text-xs lg:text-lg font-semibold">IDR 29.000 - IDR 259.999</p>
              </div>
              <button
                class="flex items-center rounded-lg justify-center w-6 h-6 lg:w-9 lg:h-9 lg:rounded-xl bg-orange-300">
                <img src="@/assets/icon/arrow-right-1.svg" alt="">
              </button>
            </div>
          </div>
          <div class="rounded-3xl flex items-end mb-4 md:w-[60%] lg:mb-0 lg:h-[415px] lg:w-[427px]">
            <img class="rounded-3xl w-full lg:w-auto lg:absolute" src="@/assets/image/resto-2.png" alt="">
            <div
              class="absolute flex lg:w-fit lg:h-32 w-fit rounded-3xl justify-between items-center ml-3 mb-3 p-4 md:w-[47%] lg:p-6 z-10 lg:m-6 bg-white lg:flex">
              <div class="flex flex-col mr-8 lg:mr-[75px]">
                <div class="flex flex-row items-center">
                  <svg class="w-4 h-4 ms-1 text-yellow-500 mr-2" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                    fill="currentColor" viewBox="0 0 22 20">
                    <path
                      d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
                  </svg>
                  <p class="font-semibold text-xs lg:text-lg text-yellow-500 mr-2">5.0</p>
                  <p class="text-gray-700 text-xs lg:text-base">(3.6K+)</p>
                </div>
                <div class="flex lg:flex">
                  <h1 class="font-semibold text-base text-black mb-1 lg:mr-2">Split Ascent</h1>
                  <span class="font-semibold text-base text-black mb-1 hidden lg:flex">Restaurant</span>
                </div>
                <p class="text-gray-700 text-xs lg:text-lg font-semibold">IDR 49.999 - IDR 560.000</p>
              </div>
              <button
                class="flex items-center rounded-lg justify-center w-6 h-6 lg:w-9 lg:h-9 lg:rounded-xl bg-orange-300">
                <img src="@/assets/icon/arrow-right-1.svg" alt="">
              </button>
            </div>
          </div>
          <div class="rounded-3xl flex items-end md:w-[60%] lg:h-[415px] lg:w-[427px] ">
            <img class="rounded-3xl w-full lg:w-auto lg:absolute" src="@/assets/image/resto-3.png" alt="">
            <div
              class="absolute flex lg:w-fit lg:h-32 w-fit rounded-3xl justify-between items-center ml-3 mb-3 p-4 md:w-[47%] lg:p-6 z-10 lg:m-6 bg-white lg:flex">
              <div class="flex flex-col mr-8 lg:mr-[75px]">
                <div class="flex flex-row items-center">
                  <svg class="w-4 h-4 ms-1 text-yellow-500 mr-2" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                    fill="currentColor" viewBox="0 0 22 20">
                    <path
                      d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
                  </svg>
                  <p class="font-semibold text-xs lg:text-lg text-yellow-500 mr-2">5.0</p>
                  <p class="text-gray-700 text-xs lg:text-base">(11K+)</p>
                </div>
                <div class="flex lg:flex">
                  <h1 class="font-semibold text-base text-black mb-1 lg:mr-2">Daza Fracture</h1>
                  <span class="font-semibold text-base text-black mb-1 hidden lg:flex">Restaurant</span>
                </div>
                <p class="text-gray-700 text-xs lg:text-lg font-semibold">IDR 29.999 - IDR 560.000</p>
              </div>
              <button
                class="flex items-center rounded-lg justify-center w-6 h-6 lg:w-9 lg:h-9 lg:rounded-xl bg-orange-300">
                <img src="@/assets/icon/arrow-right-1.svg" alt="">
              </button>
            </div>
          </div>
        </div>
        <div class="w-full flex items-center justify-center">
          <button class="w-fit h-11 lg:h-14 bg-orange-300 rounded-xl p-4 flex items-center justify-center px-7 py-4">
            <p class="font-semibold text-xs lg:text-base text-black mr-2">View All Restaurant</p>
            <img src="@/assets/icon/arrow.svg" class="w-2 h-2" alt="">
          </button>
        </div>
      </div>
      <div class="flex flex-col p-8 gap-12 lg:pl-32 lg:pr-16 lg:pb-40 lg:gap-28 lg:flex-row">
        <div class="rounded-3xl md:relative lg:relative">
          <img src="@/assets/image/chef.png" class="rounded-3xl mb-6 lg:mb-0" alt="">
          <div class="flex flex-col mb-4 items-center lg:mb-0">
            <div
              class="w-fit lg:w-44 lg:h-52 md:w-48 md:h-60 mb-6 p-6 rounded-3xl md:absolute md:left-[65%] md:bottom-[60%] lg:absolute lg:left-[75%] lg:bottom-[70%] z-99 bg-white flex flex-col items-center justify-center lg:p-0 lg:mb-0">
              <div class="lg:w-20 lg:h-20 rounded-full bg-orange-100 flex items-center justify-center mb-3">
                <img src="@/assets/icon/experience.svg" class="w-12 h-12" alt="">
              </div>
              <p class="font-semibold lg:text-lg text-gray-700 w-fit">12 Years</p>
              <p class="lg:text-base text-green-700">Experience</p>
            </div>
            <div
              class="lg:w-80 lg:h-44 md:w-80 md:h-44 w-full rounded-3xl md:absolute md:left-[50%] md:bottom-[10%] lg:absolute lg:left-[-10%] lg:bottom-[5%] bg-white p-6 flex items-center">
              <div class="w-24 h-32 rounded-xl object-cover">
                <img src="@/assets/image/bg-2.png" class="rounded-xl h-32 w-full" alt="">
              </div>
              <div class="flex flex-col h-fit ml-4">
                <p class="lg:text-base text-gray-700">Chef at restaurant:</p>
                <p class="font-semibold lg:text-lg text-gray-900 mb-4">Pearl Dolphin</p>
                <button class="flex">
                  <p class="font-semibold lg:text-base text-orange-300">View Details</p>
                  <img src="@/assets/icon/arrow-right-orange-1.svg" alt="">
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="flex flex-col w-full lg:w-[50%] justify-between items-center lg:items-start">
          <div class="flex flex-col mb-8">
            <p class="font-semibold text-xs lg:text-base mb-2 text-indigo-700 lg:mb-3 text-center lg:text-start">
              RESTAURANT BASED BY CITY</p>
            <h1 class="font-semibold text-base lg:text-3xl text-gray-900 text-center lg:text-start">Restaurant Near You
            </h1>
          </div>
          <div class="flex lg:h-36 w-full p-6 rounded-3xl bg-white justify-between mb-5">
            <div class="flex flex-col justify-between">
              <p class="font-medium text-xs lg:text-base text-green-700">PIZZA</p>
              <h1 class="font-semibold text-base lg:text-xl text-gray-900">Phoenix Satcheup</h1>
              <div class="flex">
                <img src="@/assets/icon/location.svg" class="w-4 h-4 lg:w-6 lg:h-6" alt="">
                <p class="font-medium text-xs lg:text-base text-gray-600 ml-1 lg:ml-2">Jakarta, Indonesia</p>
              </div>
            </div>
            <div class="flex items-center">
              <p class="font-medium text-xs lg:text-base text-orange-300">Profile Details</p>
              <img src="@/assets/icon/arrow-right-orange-1.svg" class="w-6 h-6" alt="">
            </div>
          </div>
          <div class="flex lg:h-36 w-full p-6 rounded-3xl justify-between mb-5">
            <div class="flex flex-col justify-between">
              <p class="font-medium text-xs lg:text-base text-green-700">VEGAN</p>
              <h1 class="font-semibold text-base lg:text-xl text-gray-900">Chamber Botfrag</h1>
              <div class="flex">
                <img src="@/assets/icon/location.svg" class="w-4 h-4 lg:w-6 lg:h-6" alt="">
                <p class="font-medium text-xs lg:text-base text-gray-600 ml-1 lg:ml-2">Jakarta, Indonesia</p>
              </div>
            </div>
          </div>
          <div class="flex lg:h-36 w-full p-6 rounded-3xl justify-between mb-5">
            <div class="flex flex-col justify-between">
              <p class="font-medium text-xs lg:text-base text-green-700">ROAST CHICKEN</p>
              <h1 class="font-semibold text-base lg:text-xl text-gray-900">Asep Vandal</h1>
              <div class="flex">
                <img src="@/assets/icon/location.svg" class="w-4 h-4 lg:w-6 lg:h-6" alt="">
                <p class="font-medium text-xs lg:text-base text-gray-600 ml-1 lg:ml-2">Jakarta, Indonesia</p>
              </div>
            </div>
          </div>
          <div class="flex lg:h-36 w-full p-6 rounded-3xl justify-between mb-5">
            <div class="flex flex-col justify-between">
              <p class="font-medium text-xs lg:text-base text-green-700">BEEF STEAK</p>
              <h1 class="font-semibold text-base lg:text-xl text-gray-900">I Made Invoker</h1>
              <div class="flex">
                <img src="@/assets/icon/location.svg" class="w-4 h-4 lg:w-6 lg:h-6" alt="">
                <p class="font-medium text-xs lg:text-base text-gray-600 ml-1 lg:ml-2">Jakarta, Indonesia</p>
              </div>
            </div>
        </div>
        <button class="w-fit lg:h-14 bg-orange-300 rounded-xl p-4 flex items-center justify-center px-7 py-4">
          <p class="font-semibold text-xs lg:text-base text-black mr-2">View All Chef</p>
          <img src="@/assets/icon/arrow.svg" class="w-2 h-2" alt="">
        </button>
      </div>
    </div>
  </body>
</main>
</template>
