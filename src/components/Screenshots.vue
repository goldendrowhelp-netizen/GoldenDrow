<template>

<section id="screenshots"
class="py-10 bg-[#09080E] overflow-hidden">

<div
class="max-w-7xl mx-auto px-6">

<!-- Heading -->

<div
class="text-center">

<span
class="inline-block
px-5
py-2
rounded-full
bg-violet-600/20
text-violet-300">

APP SCREENSHOTS

</span>

<h2
class="mt-6
text-5xl
font-black">

Beautiful Interface

</h2>

<p
class="mt-5
text-gray-400
max-w-2xl
mx-auto">

Modern Design
Easy Navigation
Premium Experience

</p>

</div>

<!-- Slider -->

<Swiper

:modules="modules"

:slides-per-view="1.2"

:centeredSlides="true"

:space-between="25"

:loop="true"

:autoplay="{

delay:2500,

disableOnInteraction:false

}"

:breakpoints="{

768:{slidesPerView:2.2},

1024:{slidesPerView:3.2},

1400:{slidesPerView:4}

}"

class="mt-20"

>

<SwiperSlide
v-for="image in images"
:key="image">

<div
class="rounded-[35px]
overflow-hidden
bg-white/5
border
border-white/10
hover:scale-105
transition">

<img
:src="image"
class="w-full">

</div>

</SwiperSlide>

</Swiper>

</div>

</section>

</template>

<script setup>

import { Swiper, SwiperSlide } from "swiper/vue";

import { Autoplay } from "swiper/modules";

import "swiper/css";

const modules=[Autoplay];

const images=[

"/src/assets/screenshots/screen1.jpeg",

"/src/assets/screenshots/screen2.jpeg",

"/src/assets/screenshots/screen3.jpeg",

"/src/assets/screenshots/screen4.jpeg",

"/src/assets/screenshots/screen5.jpeg",

"/src/assets/screenshots/screen6.jpeg",

];

</script>