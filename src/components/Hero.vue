<template>

<section id = "home"
class="relative min-h-screen overflow-hidden bg-[#09080E] flex items-center">

    <!-- Background Image -->

    <div class="absolute inset-0">

        <img
        src="/src/assets/banner_lottery.png"
        alt="GoldenDrow Banner"
        class="w-full h-full object-cover object-center select-none">

    </div>

    <!-- Overlay -->

    <div
    class="absolute inset-0
    bg-gradient-to-r
    from-[#09080E]/95
    via-[#09080E]/75
    to-[#09080E]/20">

    </div>

    <!-- Purple Glow -->

    <div
    class="absolute
    -left-52
    top-24
    w-[550px]
    h-[550px]
    rounded-full
    bg-violet-700/20
    blur-[180px]">

    </div>

    <!-- Gold Glow -->

    <div
    class="absolute
    right-0
    bottom-0
    w-[450px]
    h-[450px]
    rounded-full
    bg-yellow-400/10
    blur-[200px]">

    </div>

    <!-- Content -->

    <div
    class="relative
    z-20
    max-w-7xl
    mx-auto
    px-6
    lg:px-8
    w-full">

        <div class="max-w-2xl">

            <!-- Badge -->

            <div
            class="inline-flex
            items-center
            gap-3
            rounded-full
            border
            border-yellow-500/20
            bg-white/5
            backdrop-blur-xl
            px-6
            py-3">

                <span
                class="w-2.5
                h-2.5
                rounded-full
                bg-yellow-400
                animate-pulse">

                </span>

                <span
                class="text-yellow-400
                font-medium">

                    Premium Lottery Platform

                </span>

            </div>

            <!-- Heading -->

            <h1
            class="mt-8
            text-5xl
            md:text-6xl
            xl:text-8xl
            font-black
            leading-[0.95]
            tracking-tight">

                PLAY

                <br>

                LOTTERY

                <br>

                WIN BIG

                <br>

                EVERYDAY

            </h1>

            <!-- Description -->

            <p
            class="mt-8
            max-w-xl
            text-lg
            text-gray-300
            leading-9">

                Experience the next generation lottery platform with secure wallet, instant draw results, fair gameplay and exciting daily rewards.

            </p>

            <!-- Buttons -->

            <div
            class="flex
            flex-wrap
            gap-5
            mt-10">

                <a

                href="/apk/GoldenDrow.apk"

                download

                class="inline-flex

                items-center

                justify-center

                h-14

                px-10

                rounded-full

                bg-violet-600

                hover:bg-violet-700

                transition-all

                duration-300

                shadow-[0_0_40px_rgba(124,58,237,.45)]">

                    Download APK

                </a>

                <a

                href="#features"

                class="inline-flex

                items-center

                justify-center

                h-14

                px-10

                rounded-full

                border

                border-white/10

                bg-white/5

                backdrop-blur-xl

                hover:border-yellow-400

                transition">

                    Learn More

                </a>

            </div>

                        <!-- Statistics -->

            <div
                class="grid grid-cols-2 md:grid-cols-4 gap-5 mt-16">

                <div
                    class="rounded-3xl border border-white/10 bg-white/5 backdrop-blur-xl p-6 hover:border-violet-500 transition">

                    <h2 class="text-3xl font-bold text-yellow-400">
                        120K+
                    </h2>

                    <p class="mt-2 text-gray-400">
                        Active Players
                    </p>

                </div>

                <div
                    class="rounded-3xl border border-white/10 bg-white/5 backdrop-blur-xl p-6 hover:border-violet-500 transition">

                    <h2 class="text-3xl font-bold text-yellow-400">
                        ৳15M+
                    </h2>

                    <p class="mt-2 text-gray-400">
                        Prize Paid
                    </p>

                </div>

                <div
                    class="rounded-3xl border border-white/10 bg-white/5 backdrop-blur-xl p-6 hover:border-violet-500 transition">

                    <h2 class="text-3xl font-bold text-yellow-400">
                        24/7
                    </h2>

                    <p class="mt-2 text-gray-400">
                        Live Support
                    </p>

                </div>

                <div
                    class="rounded-3xl border border-white/10 bg-white/5 backdrop-blur-xl p-6 hover:border-violet-500 transition">

                    <h2 class="text-3xl font-bold text-yellow-400">
                        99.9%
                    </h2>

                    <p class="mt-2 text-gray-400">
                        Secure System
                    </p>

                </div>

            </div>

        </div>

    </div>

    <!-- Scroll Down -->

    <div
        class="absolute bottom-8 left-1/2 -translate-x-1/2 animate-bounce z-30">

        <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-8 h-8 text-yellow-400"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor">

            <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M12 5v14m0 0l-5-5m5 5l5-5"/>

        </svg>

    </div>

</section>
</template>

<script setup>

// Hero Section

</script>