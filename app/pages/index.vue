<script setup lang="ts">
import WorksGrid from "../components/WorksGrid.vue";
</script>

<template>
  <main class="flex flex-col items-center gap-20">
    <!-- HERO -->
    <section
      class="w-full lg:max-w-7xl min-h-[calc(100dvh-4rem)] lg:min-h-[calc(100dvh-5rem)] flex flex-col justify-center border-b-2 border-white mx-auto"
    >
      <div
        class="grid sm:bg-amber-900 md:bg-red-950 lg:bg-green-900 xl:bg-red-800 lg:grid-cols-4 lg:grid-rows-4 place-items-center lg:place-items-start gap-4 lg:gap-4 text-center text-white border-2"
      >
        <h1
          class="lg:col-start-1 lg:col-end-4 border-2 text-3xl sm:text-4xl md:text-5xl lg:text-6xl xl:text-7xl font-semibold"
        >
          ILHAM DWI PAMBUDI
        </h1>
        <h2
          class="sm:text-3xl md:text-4xl lg:col-start-1 lg:col-end-4 border-2 text-2xl lg:text-6xl"
        >
          Full-Stack Developer
        </h2>

        <div
          class="lg:col-start-4 lg:row-start-1 lg:row-end-5 lg:place-self-center border-2 h-60 w-60 md:h-70 md:w-70 xl:h-70 xl:w-70 rounded-full overflow-hidden"
        >
          <NuxtImg class="h-full w-full object-cover" src="/avatar.jpg" />
        </div>

        <div
          class="text-base lg:col-start-1 lg:col-end-4 border-2 lg:text-left lg:max-w-2xl"
        >
          <p
            class="max-w-xl text-base sm:text-lg sm:text-normal lg:max-w-2xl lg:text-xl"
          >
            A passionate web developer focused on building modern and meaningful
            digital experiences.
          </p>
        </div>
        <button
          class="rounded-xl border px-4 py-2 hover:bg-white hover:text-black transition"
        >
          Learn More
        </button>
      </div>
    </section>
    <!-- EXPERTISE -->
    <section
      id="expertise"
      class="flex flex-col sm:items-center gap-6 border-2 mx-auto bg-amber-500 items-center"
    >
      <Expertise />
    </section>
    <!-- WORKS -->
    <section
      id="works"
      class="flex justify-center items-center flex-col border-2 w-full gap-10"
    >
      <WorksGrid />
    </section>
    <!-- JOURNEY -->
    <section class="flex flex-col items-center gap-8 border-2">
      <Journey />
    </section>
    <!-- CONTACT -->
    <section class="w-11/12 md:w-full grid md:grid-cols-2 max-w-7xl md:gap-10 lg:gap-15">
      <div class="border-2 flex flex-col gap-4">
        <h2 class="text-3xl lg:text-4xl font-bold">Let's Work Together</h2>
        <p>
          I'm open to new opportunities, collaborations, and meaningful
          projects. Let's connect and build something great.
        </p>
        <ul>
          <li class="flex items-center gap-2">
            <div class="flex justify-center items-center w-10 h-10  bg-white/20 backdrop-blur-md shadow-lg transition duration-200 rounded-lg">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="none"
                class="w-8 h-8"
              >
                <rect
                  x="3"
                  y="5"
                  width="18"
                  height="14"
                  rx="1.5"
                  stroke="white"
                  stroke-width="2"
                />
                <path
                  d="M4 7l8 6 8-6"
                  stroke="white"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
            </div>
            <div>
              <p class="font-bold">Email</p>
              <p>Iamsamuelilham@gmail.com</p>
            </div>
          </li>
          <li class="flex items-center gap-2">
            <div class="flex justify-center items-center w-10 h-10  bg-white/20 backdrop-blur-md shadow-lg transition duration-200 rounded-lg">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="none"
                class="w-8 h-8"
              >
                <path
                  d="M12 21s7-5.8 7-12a7 7 0 1 0-14 0c0 6.2 7 12 7 12Z"
                  stroke="white"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <circle
                  cx="12"
                  cy="9"
                  r="2.5"
                  stroke="white"
                  stroke-width="2"
                />
              </svg>
            </div>
            <div>
              <p class="font-bold">Location</p>
              <p>West Jakarta, Indonesia</p>
            </div>
          </li>
        </ul>
        <div class="flex flex-col">
          <p class="text-lg font-bold">Find me on</p>

          <div class="flex gap-2">
            <div class="flex justify-center gap-1 lg:justify-start">
              <!-- INSTAGRAM -->
              <a
                href="https://www.instagram.com/iamsamuelilham?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw=="
                target="_blank"
                rel="noopener noreferrer"
                class="flex h-10 w-30 items-center justify-center gap-2 rounded-lg bg-white/20 px-3 backdrop-blur-md shadow-lg transition duration-200 hover:bg-white/30 hover:-translate-y-0.5"
              >
                <svg
                  class="h-6 w-6 shrink-0"
                  viewBox="4 4 24 24"
                  fill="currentColor"
                  xmlns="http://www.w3.org/2000/svg"
                  aria-hidden="true"
                >
                  <path
                    d="M22.3,8.4c-0.8,0-1.4,0.6-1.4,1.4c0,0.8,0.6,1.4,1.4,1.4c0.8,0,1.4-0.6,1.4-1.4C23.7,9,23.1,8.4,22.3,8.4z"
                  />
                  <path
                    d="M16,10.2c-3.3,0-5.9,2.7-5.9,5.9s2.7,5.9,5.9,5.9s5.9-2.7,5.9-5.9S19.3,10.2,16,10.2z M16,19.9c-2.1,0-3.8-1.7-3.8-3.8
            c0-2.1,1.7-3.8,3.8-3.8c2.1,0,3.8,1.7,3.8,3.8C19.8,18.2,18.1,19.9,16,19.9z"
                  />
                  <path
                    d="M20.8,4h-9.5C7.2,4,4,7.2,4,11.2v9.5c0,4,3.2,7.2,7.2,7.2h9.5c4,0,7.2-3.2,7.2-7.2v-9.5C28,7.2,24.8,4,20.8,4z M25.7,20.8
            c0,2.7-2.2,5-5,5h-9.5c-2.7,0-5-2.2-5-5v-9.5c0-2.7,2.2-5,5-5h9.5c2.7,0,5,2.2,5,5V20.8z"
                  />
                </svg>
                <span class="text-sm font-bold">Instagram</span>
              </a>

              <!-- LINKEDIN -->
              <a
                href="https://www.linkedin.com/in/ilham-dwi-pambudi-0a3458171/"
                target="_blank"
                rel="noopener noreferrer"
                class="flex h-10 w-30 items-center justify-center gap-2 rounded-lg bg-white/20 px-3 backdrop-blur-md shadow-lg transition duration-200 hover:bg-white/30 hover:-translate-y-0.5"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="h-6 w-6 shrink-0"
                  aria-hidden="true"
                >
                  <path
                    d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"
                  ></path>
                  <rect width="4" height="12" x="2" y="9"></rect>
                  <circle cx="4" cy="4" r="2"></circle>
                </svg>
                <span class="text-sm font-bold">LinkedIn</span>
              </a>
            </div>
          </div>
        </div>
      </div>
      <AppForm />
    </section>
  </main>
</template>
