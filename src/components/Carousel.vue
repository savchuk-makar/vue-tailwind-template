<template>
  <section class="bg-white max-w-screen-lg mx-auto" id="block3">
    <div class="bg-white">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
          <p
            class="text-4xl font-extrabold text-gray-900 sm:text-5xl sm:tracking-tight lg:text-6xl"
          >
            Инфраструктура
          </p>
        </div>
      </div>
    </div>
    <div
      class="gap-8 items-center py-8 px-4 mx-auto max-w-screen-xl xl:gap-16 md:grid md:grid-cols-3 sm:py-16 lg:px-6"
    >
      <ul class="max-w-md space-y-1 text-gray-500 list-inside dark:text-gray-400 col-span-1">
        <li class="flex items-center">
          <svg
            class="w-3.5 h-3.5 mr-2 text-green-500 dark:text-green-400 flex-shrink-0"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            viewBox="0 0 20 20"
          >
            <path
              d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
            />
          </svg>
          Ozon
        </li>
        <li class="flex items-center">
          <svg
            class="w-3.5 h-3.5 mr-2 text-green-500 dark:text-green-400 flex-shrink-0"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            viewBox="0 0 20 20"
          >
            <path
              d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
            />
          </svg>
          Wildberries
        </li>
        <li class="flex items-center">
          <svg
            class="w-3.5 h-3.5 mr-2 text-green-500 dark:text-green-400 flex-shrink-0"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            viewBox="0 0 20 20"
          >
            <path
              d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
            />
          </svg>
          Магнит
        </li>
        <li class="flex items-center">
          <svg
            class="w-3.5 h-3.5 mr-2 text-green-500 dark:text-green-400 flex-shrink-0"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            viewBox="0 0 20 20"
          >
            <path
              d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
            />
          </svg>
          Пятёрочка
        </li>
        <li class="flex items-center">
          <svg
            class="w-3.5 h-3.5 mr-2 text-green-500 dark:text-green-400 flex-shrink-0"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            viewBox="0 0 20 20"
          >
            <path
              d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
            />
          </svg>
          Удачный (сеть фермерских магазинов)
        </li>
      </ul>

      <div class="col-span-2">
        <swiper
          :modules="modules"
          :slides-per-view="1"
          :space-between="20"
          navigation
          :pagination="{ clickable: true }"
          :free-mode="true"
          @swiper="onSwiper"
        >
          <swiper-slide>
            <img src="@/assets/img/ozon.jpg" class="object-conver w-full rounded-lg" />
          </swiper-slide>
          <swiper-slide>
            <img src="@/assets/img/sber.jpg" class="object-conver w-full rounded-lg" />
          </swiper-slide>
          <swiper-slide>
            <img src="@/assets/img/dac.jpg" class="object-conver w-full rounded-lg" />
          </swiper-slide>
          <swiper-slide>
            <img src="@/assets/img/magnit.jpg" class="object-conver w-full rounded-lg" />
          </swiper-slide>
          <swiper-slide>
            <img src="@/assets/img/russia.jpg" class="object-conver w-full rounded-lg" />
          </swiper-slide>
        </swiper>
      </div>
    </div>
  </section>

  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8"></div>
</template>

<script setup>
// import Swiper core and required modules
import { Navigation, Pagination, A11y } from "swiper/modules";

// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";
import "swiper/css/navigation";
import "swiper/css/pagination";
import "swiper/css/scrollbar";
const onSwiper = (swiper) => {
  console.log(swiper);
};
const modules = [Navigation, Pagination, A11y];
</script>
