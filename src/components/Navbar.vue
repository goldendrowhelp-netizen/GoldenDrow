<template>
  <header
    :class="[
      'fixed top-0 left-0 w-full z-50 transition-all duration-300',
      isScrolled
        ? 'bg-[#09080E]/90 backdrop-blur-xl border-b border-white/10'
        : 'bg-transparent'
    ]"
  >
    <div
      class="max-w-7xl mx-auto h-20 px-6 lg:px-8 flex items-center justify-between"
    >
      <!-- Logo -->
      <a href="#home" @click.prevent="scrollToSection('#home')">
        <img
          src="/src/assets/logo.png"
          alt="GoldenDrow"
          class="h-14"
        />
      </a>

      <!-- Desktop Menu -->
      <nav class="hidden lg:flex items-center gap-8">

        <a
          v-for="item in menuItems"
          :key="item.id"
          href="#"
          @click.prevent="scrollToSection(item.id)"
          class="text-white hover:text-yellow-400 transition"
        >
          {{ item.name }}
        </a>

      </nav>

      <!-- Download Button -->

      <a
        href="#"
        @click.prevent="scrollToSection('#download')"
        class="hidden lg:flex items-center justify-center px-8 h-12 rounded-full bg-violet-600 hover:bg-violet-700 transition"
      >
        Download APK
      </a>

      <!-- Mobile Menu Button -->

      <button
        @click="mobileMenu = !mobileMenu"
        class="lg:hidden text-3xl"
      >
        ☰
      </button>

    </div>

    <!-- Mobile Menu -->

    <transition
      enter-active-class="duration-300 ease-out"
      leave-active-class="duration-200 ease-in"
      enter-from-class="opacity-0 -translate-y-5"
      enter-to-class="opacity-100 translate-y-0"
      leave-from-class="opacity-100 translate-y-0"
      leave-to-class="opacity-0 -translate-y-5"
    >

      <div
        v-if="mobileMenu"
        class="lg:hidden bg-[#111018]/95 backdrop-blur-xl border-t border-white/10"
      >

        <nav class="flex flex-col p-6 gap-5">

          <a
            v-for="item in menuItems"
            :key="item.id"
            href="#"
            @click.prevent="scrollToSection(item.id)"
            class="text-white hover:text-yellow-400 transition"
          >
            {{ item.name }}
          </a>

          <a
            href="#"
            @click.prevent="scrollToSection('#download')"
            class="flex justify-center items-center h-12 rounded-full bg-violet-600 hover:bg-violet-700"
          >
            Download APK
          </a>

        </nav>

      </div>

    </transition>

  </header>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";

const mobileMenu = ref(false);
const isScrolled = ref(false);

const menuItems = [
  { name: "Home", id: "#home" },
  { name: "Features", id: "#features" },
  { name: "Statistics", id: "#statistics" },
  { name: "Screenshots", id: "#screenshots" },
  { name: "Download", id: "#download" },
  { name: "FAQ", id: "#faq" },
  
];

function scrollToSection(id) {
  mobileMenu.value = false;

  const section = document.querySelector(id);

  if (section) {
    section.scrollIntoView({
      behavior: "smooth",
      block: "start",
    });
  }
}

const handleScroll = () => {
  isScrolled.value = window.scrollY > 30;
};

onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});

onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>