<!--
  This example requires Tailwind CSS v2.0+ 
  
  This example requires some changes to your config:
  
  ```
  // tailwind.config.js
  module.exports = {
    // ...
    plugins: [
      // ...
      require('@tailwindcss/forms'),
    ],
  }
  ```
-->
<template>
    <div class="bg-gray-100" id="contacts">
      <div class="max-w-7xl mx-auto py-16 px-4 sm:py-24 sm:px-6 lg:px-8">
        <div class="relative bg-white shadow-xl">
          <h2 class="sr-only">Contact us</h2>
  
            <!-- Contact information -->
            <div class="relative overflow-hidden py-10 px-6 bg-emerald-600 sm:px-10 xl:p-12">
              <div class="absolute inset-0 pointer-events-none sm:hidden" aria-hidden="true">
                <svg class="absolute inset-0 w-full h-full" width="343" height="388" viewBox="0 0 343 388" fill="none" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
                  <path d="M-99 461.107L608.107-246l707.103 707.107-707.103 707.103L-99 461.107z" fill="url(#linear1)" fill-opacity=".1" />
                  <defs>
                    <linearGradient id="linear1" x1="254.553" y1="107.554" x2="961.66" y2="814.66" gradientUnits="userSpaceOnUse">
                      <stop stop-color="#fff" />
                      <stop offset="1" stop-color="#fff" stop-opacity="0" />
                    </linearGradient>
                  </defs>
                </svg>
              </div>
              <div class="hidden absolute top-0 right-0 bottom-0 w-1/2 pointer-events-none sm:block lg:hidden" aria-hidden="true">
                <svg class="absolute inset-0 w-full h-full" width="359" height="339" viewBox="0 0 359 339" fill="none" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
                  <path d="M-161 382.107L546.107-325l707.103 707.107-707.103 707.103L-161 382.107z" fill="url(#linear2)" fill-opacity=".1" />
                  <defs>
                    <linearGradient id="linear2" x1="192.553" y1="28.553" x2="899.66" y2="735.66" gradientUnits="userSpaceOnUse">
                      <stop stop-color="#fff" />
                      <stop offset="1" stop-color="#fff" stop-opacity="0" />
                    </linearGradient>
                  </defs>
                </svg>
              </div>
              <div class="hidden absolute top-0 right-0 bottom-0 w-1/2 pointer-events-none lg:block" aria-hidden="true">
                <svg class="absolute inset-0 w-full h-full" width="160" height="678" viewBox="0 0 160 678" fill="none" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
                  <path d="M-161 679.107L546.107-28l707.103 707.107-707.103 707.103L-161 679.107z" fill="url(#linear3)" fill-opacity=".1" />
                  <defs>
                    <linearGradient id="linear3" x1="192.553" y1="325.553" x2="899.66" y2="1032.66" gradientUnits="userSpaceOnUse">
                      <stop stop-color="#fff" />
                      <stop offset="1" stop-color="#fff" stop-opacity="0" />
                    </linearGradient>
                  </defs>
                </svg>
              </div>
              <h3 class="text-lg font-medium text-white">Контактная информация</h3>
              <p class="mt-6 text-base text-indigo-50 max-w-4xl">
С вами будут работать профессиональные специалисты. Вам помогут выбрать участок, при необходимости оформить ипотеку. Вы сможете уточнить любые правовые вопросы, связанные с оформлением в собственность. Наши специалисты бесплатно сопроводят вас на всех этапах сделки от момента выбора, до получения права собственности. Так же мы рады помочь нашим покупателям в дальнейших возникающих вопросах. Например как оформить свет, газ, как получить милицейский адрес участка, к кому обратиться со скважиной, вопросы по подрядным организациям по строительству дома. Будем рады помочь и не бросаем наших покупателей.</p>
              <dl class="mt-8 space-y-6">
                <dt><span class="sr-only">Phone number</span></dt>
                <dd class="flex text-base text-indigo-50">
                  <PhoneIcon class="flex-shrink-0 w-6 h-6 text-indigo-200" aria-hidden="true" />
                  <a href="tel:+78126607060"> +7 812 660 70 60</a>
                </dd>
                <dt><span class="sr-only">Email</span></dt>
                <dd class="flex text-base text-indigo-50">
                  <MailIcon class="flex-shrink-0 w-6 h-6 text-indigo-200" aria-hidden="true" />
                  <a href="mailto:support@largeland.ru">support@largeland.ru</a>
                </dd>
              </dl>
            </div>
  
            <!-- Contact form -->
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import { MailIcon, PhoneIcon } from '@heroicons/vue/outline'
  
  export default {
    components: {
      MailIcon,
      PhoneIcon,
    },
  }
  </script>