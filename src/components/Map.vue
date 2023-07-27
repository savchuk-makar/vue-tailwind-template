<template>
<section class="bg-white" id="map">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
          <p
            class="text-4xl font-extrabold text-gray-900 sm:text-5xl sm:tracking-tight lg:text-6xl"
          >
          Местоположение
          </p>
        </div>
        <div class="rounded-md bg-indigo-50 p-4 mt-4">
            <div class="flex">
            <div class="flex-shrink-0">
                <InformationCircleIcon class="h-5 w-5 text-indigo-400" aria-hidden="true" />
            </div>
            <div class="ml-3">
                <h3 class="text-sm font-medium text-indigo-800">Транспортная доступность:</h3>
                <div class="mt-2 text-sm text-indigo-700">
                <p>
                    Киевское шоссе одно из самых разгруженных дорог, в сравнении с другими шоссе.  Доехать в поселок можно 3 мя способами:
                    <ul>
                        <li>
                            -На автомобиле
                        </li>
                        <li>
                            -по Железной дороге, с Балтийского вокзала, станция Сиверская, от туда идут автобусы № 500, № 121Т, № 41А-003, в дороге 15 минут(11 км)
                        </li>
                        <li>
                            — на маршрутке из Санкт-Петербурга:
                            <ol>
                             <li>
                                от  м. Московская маршрутное такси № 100 до остановки Гатчина Варшавский вокзал, далее автобус № 531 до остановки «Рождествено центр».
                             </li>
                             <li>
                                от  м. Московская маршрутное такси № 100 до остановки Гатчина Варшавский вокзал, далее маршрутное такси № 151 до станции Сиверская, далее автобус № 500 или маршрутное такси № 121 до остановки «Рождествено центр».
                             </li>
                            </ol>
                        </li>
                    </ul>
     
    


                </p>
              
                </div>
            </div>
            </div>
        </div>
      </div>
    <div class="gap-8 items-center py-8 px-4 mx-auto max-w-screen-xl xl:gap-16 md:grid md:grid-cols-1 sm:py-16 lg:px-6">
        <YandexMap :settings="settings" :coordinates="[29.957701, 59.324734]" class="w-full h-[600px]" :zoom="13" :controls="['zoom']">
            <!--Markers-->
        </YandexMap>        
    </div>
</section>
</template>
<script setup>
import { YandexMap } from 'vue-yandex-maps'
import {InformationCircleIcon} from "@heroicons/vue/outline"
const settings = {
    apiKey: '', // Индивидуальный ключ API
    lang: 'ru_RU', // Используемый язык
    coordorder: 'longlat', // Порядок задания географических координат
    debug: false, // Режим отладки
    version: '2.1' // Версия Я.Карт
};
</script>

