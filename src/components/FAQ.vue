<template>
<section id="faq" class="py-18 bg-[#0B0B10]">

<div class="max-w-5xl mx-auto px-6">

<!-- Heading -->

<div class="text-center">

<span
class="inline-flex
px-5
py-2
rounded-full
bg-violet-600/20
text-violet-300">

FAQ

</span>

<h2
class="mt-6
text-5xl
font-black">

Frequently Asked Questions

</h2>

<p
class="mt-5
text-gray-400">

Everything you need to know about GoldenDrow.

</p>

</div>

<!-- FAQ -->

<div
class="mt-16
space-y-5">

<div
v-for="(item,index) in faqs"
:key="index"
class="rounded-3xl
border
border-white/10
bg-white/5
backdrop-blur-xl
overflow-hidden">

<button

@click="toggle(index)"

class="w-full
flex
justify-between
items-center
p-6
text-left">

<span
class="text-xl
font-semibold">

{{item.question}}

</span>

<span
class="text-3xl">

{{openIndex===index ? '−' : '+'}}

</span>

</button>

<div

v-show="openIndex===index"

class="px-6
pb-6
text-gray-400
leading-8">

{{item.answer}}

</div>

</div>

</div>

</div>

</section>
</template>

<script setup>

import { ref } from "vue";

const openIndex = ref(0);

const toggle=(index)=>{

openIndex.value=openIndex.value===index?-1:index;

}

const faqs=[

{

question:"How do I download the APK?",

answer:"Click the Download APK button and install the latest version on your Android device."

},

{

question:"Is GoldenDrow free?",

answer:"Yes. Downloading and installing the application is free."

},

{

question:"How secure is my account?",

answer:"Your account uses encrypted communication and secure authentication."

},

{

question:"How do I contact support?",

answer:"Use the Contact section or our official support channel."

},

{

question:"Does the app receive updates?",

answer:"Yes. We regularly release improvements and new features."

}

];

</script>