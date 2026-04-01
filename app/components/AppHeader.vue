<script setup>
const isNavOpen = ref(false);

const toggleNav = () => {
  isNavOpen.value = !isNavOpen.value;
};
</script>

<template>
  <header class="sticky top-0 z-50">
    <nav
      class="relative z-50 h-16 lg:h-20 lg:flex lg:flex-col justify-center bg-black"
    >
      <ul
        class="md:hidden relative z-20 h-full flex justify-between px-4 border-2 border-white bg-black text-white items-center"
      >
        <li class="text-3xl">
          <NuxtLink to="/">IP</NuxtLink>
        </li>

        <li class="flex items-center">
          <button
            class="group inline-flex h-12 w-12 items-center justify-center rounded border-2 bg-black text-center text-white transition"
            :aria-pressed="isNavOpen"
            @click="toggleNav"
          >
            <span class="sr-only">
              {{ isNavOpen ? "Close menu" : "Open menu" }}
            </span>

            <svg
              class="pointer-events-none h-6 w-6 fill-current"
              viewBox="0 0 16 16"
              xmlns="http://www.w3.org/2000/svg"
            >
              <rect
                class="origin-center -translate-y-[5px] translate-x-[7px] transition-all duration-300 ease-[cubic-bezier(.5,.85,.25,1.1)] group-[[aria-pressed=true]]:translate-x-0 group-[[aria-pressed=true]]:translate-y-0 group-[[aria-pressed=true]]:rotate-[315deg]"
                y="7"
                width="9"
                height="2"
                rx="1"
              />
              <rect
                class="origin-center transition-all duration-300 ease-[cubic-bezier(.5,.85,.25,1.8)] group-[[aria-pressed=true]]:rotate-45"
                y="7"
                width="16"
                height="2"
                rx="1"
              />
              <rect
                class="origin-center translate-y-[5px] transition-all duration-300 ease-[cubic-bezier(.5,.85,.25,1.1)] group-[[aria-pressed=true]]:translate-y-0 group-[[aria-pressed=true]]:-rotate-[225deg]"
                y="7"
                width="9"
                height="2"
                rx="1"
              />
            </svg>
          </button>
        </li>
      </ul>
      <ul
        class="hidden relative z-20 md:flex border-2 justify-center items-center bg-black md:text-xl lg:text-2xl uppercase gap-6 border-white h-full"
      >
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/about">About</NuxtLink></li>
        <li><NuxtLink to="/works">Works</NuxtLink></li>
        <li>
          <NuxtLink to="/contact">Contact</NuxtLink>
        </li>
      </ul>

      <Transition name="roll">
        <div v-if="isNavOpen" class="absolute top-full left-0 z-40 w-full">
          <ul class="flex flex-col items-center gap-4 bg-red-900 text-3xl">
            <li><NuxtLink @click="toggleNav" to="/">Home</NuxtLink></li>
            <li><NuxtLink @click="toggleNav" to="/about">About</NuxtLink></li>
            <li><NuxtLink @click="toggleNav" to="/works">Works</NuxtLink></li>
            <li>
              <NuxtLink @click="toggleNav" to="/contact">Contact</NuxtLink>
            </li>
          </ul>
        </div>
      </Transition>
    </nav>
  </header>
</template>
<style scoped>
.roll-enter-active {
  transition: all 0.3s ease-out;
}

.roll-leave-active {
  transition: all 0.3s ease-in;
}

.roll-enter-from,
.roll-leave-to {
  transform: translateY(-200px);
}
</style>
