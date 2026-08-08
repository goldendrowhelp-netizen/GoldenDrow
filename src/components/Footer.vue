<template>
  <footer id="footer" class="bg-[#09080E] border-t border-white/10">

    <div class="max-w-7xl mx-auto px-6 py-20">

      <div class="grid lg:grid-cols-4 md:grid-cols-2 gap-12">

        <!-- Logo -->

        <div>

          <img
            :src="logo"
            alt="GoldenDrow"
            class="h-16"
          >

          <p class="mt-6 text-gray-400 leading-8">

            GoldenDrow is a modern lottery platform designed with
            security, speed and premium user experience.

          </p>

        </div>

        <!-- Quick Links -->

        <div>

          <h3 class="text-xl font-bold">

            Quick Links

          </h3>

          <ul class="mt-6 space-y-4">

            <li><a href="#home" class="hover:text-yellow-400 transition">Home</a></li>

            <li><a href="#features" class="hover:text-yellow-400 transition">Features</a></li>

            <li><a href="#statistics" class="hover:text-yellow-400 transition">Statistics</a></li>

            <li><a href="#screenshots" class="hover:text-yellow-400 transition">Screenshots</a></li>

            <li><a href="#download" class="hover:text-yellow-400 transition">Download</a></li>

            <li><a href="#faq" class="hover:text-yellow-400 transition">FAQ</a></li>

          </ul>

        </div>

        <!-- Download -->

        <div>

          <h3 class="text-xl font-bold">

            Download

          </h3>

          <p class="mt-6 text-gray-400">

            Latest Version

          </p>

          <p class="mt-2 text-gray-400">

            Android APK

          </p>

          <p class="mt-2 text-gray-400">

            Version 1.0.0

          </p>

          <a
            :href="apkUrl"
            download
            class="mt-8 inline-flex items-center justify-center px-8 h-12 rounded-full bg-violet-600 hover:bg-violet-700 transition"
          >

            Download APK

          </a>

        </div>

        <!-- Legal -->

        <div>

          <h3 class="text-xl font-bold">

            Legal

          </h3>

          <ul class="mt-6 space-y-4">

            <li>

              <a href="#" class="hover:text-yellow-400 transition">

                Privacy Policy

              </a>

            </li>

            <li>

              <a href="#" class="hover:text-yellow-400 transition">

                Terms & Conditions

              </a>

            </li>

            <li>

              <a href="#" class="hover:text-yellow-400 transition">

                Disclaimer

              </a>

            </li>

          </ul>

        </div>

      </div>

      <!-- Bottom -->

      <div
        class="border-t border-white/10 mt-16 pt-8 flex flex-col lg:flex-row items-center justify-between">

        <p class="text-gray-500">

          © 2026 GoldenDrow. All Rights Reserved.

        </p>

        <button
          @click="scrollTop"
          class="mt-5 lg:mt-0 w-12 h-12 rounded-full bg-violet-600 hover:bg-violet-700 transition"
        >

          ↑

        </button>

      </div>

    </div>

  </footer>
</template>

<script setup>
import logo from "../assets/logo.png";

const apkUrl = `${import.meta.env.BASE_URL}apk/GoldenDrow.apk`;

const scrollTop = () => {
  window.scrollTo({
    top: 0,
    behavior: "smooth",
  });
};
</script>