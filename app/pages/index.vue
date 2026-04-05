<script setup lang="ts">
import WorksGrid from "../components/WorksGrid.vue";
</script>

<template>
  <main class="flex flex-col items-center gap-10">
    <!-- HERO -->
    <section
      class="w-full lg:max-w-7xl min-h-[calc(100dvh-4rem)] lg:min-h-[calc(100dvh-5rem)] flex flex-col justify-center mx-auto border-b-2"
    >
      <div
        class="grid lg:grid-cols-4 lg:grid-rows-4 place-items-center lg:place-items-start gap-4 lg:gap-4 text-center text-white"
      >
        <h1
          class="lg:col-start-1 lg:col-end-4 text-4xl sm:text-5xl md:text-6xl lg:text-6xl xl:text-7xl font-semibold leading-none"
        >
          ILHAM DWI PAMBUDI
        </h1>

        <h2
          class="text-2xl sm:text-3xl md:text-4xl lg:col-start-1 lg:col-end-4 lg:text-5xl leading-tight"
        >
          Full-Stack Developer
        </h2>

        <div
          class="lg:col-start-4 lg:row-start-1 lg:row-end-5 lg:place-self-center h-64 w-64 md:h-72 md:w-72 lg:h-72 lg:w-72 xl:h-80 xl:w-80 rounded-full overflow-hidden"
        >
          <NuxtImg class="h-full w-full object-cover" src="/avatar.jpg" />
        </div>

        <div
          class="text-base lg:col-start-1 lg:col-end-4 lg:text-left lg:max-w-2xl"
        >
          <p
            class="max-w-xl text-base sm:text-lg lg:max-w-2xl lg:text-xl leading-relaxed"
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
      class="flex flex-col sm:items-center gap-10 mx-auto items-center border-b-2 w-full max-w-7xl pb-10"
    >
      <Expertise />
    </section>
    <!-- WORKS -->
    <section
      id="works"
      class="flex justify-center items-center flex-col w-full gap-10"
    >
      <WorksGrid />
    </section>
    <!-- JOURNEY -->
    <section class="flex flex-col items-center gap-8 my-15">
      <Journey />
    </section>
    <!-- CONTACT -->
    <section
      class="w-11/12 md:w-full grid md:grid-cols-2 max-w-7xl gap-10 lg:gap-15"
    >
      <div class="flex flex-col gap-4">
        <h2 class="text-3xl lg:text-4xl font-bold">Let's Work Together</h2>
        <p>
          Whether it’s a job opportunity, a collaboration, an open-source
          initiative, or a hobby project, I’m always excited to connect and
          create something meaningful.
        </p>
        <ul class="flex flex-col gap-2">
          <li class="flex items-center gap-2">
            <div
              class="flex justify-center items-center w-12 h-12 bg-white/20 backdrop-blur-md shadow-lg transition duration-200 rounded-lg"
            >
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
            <div
              class="flex justify-center items-center w-12 h-12 bg-white/20 backdrop-blur-md shadow-lg transition duration-200 rounded-lg"
            >
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
          <p class="text-lg font-bold text-center md:text-left">Find me on</p>
          <div
            class="flex justify-center md:justify-start gap-2 lg:justify-start flex-wrap"
          >
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

            <!-- GITHUB -->
            <a
              href="https://www.linkedin.com/in/ilham-dwi-pambudi-0a3458171/"
              target="_blank"
              rel="noopener noreferrer"
              class="flex h-10 w-30 items-center justify-center gap-2 rounded-lg bg-white/20 px-3 backdrop-blur-md shadow-lg transition duration-200 hover:bg-white/30 hover:-translate-y-0.5"
            >
              <svg
                fill="#ffffff"
                viewBox="0 -0.5 25 25"
                xmlns="http://www.w3.org/2000/svg"
              >
                <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                <g
                  id="SVGRepo_tracerCarrier"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                ></g>
                <g id="SVGRepo_iconCarrier">
                  <path
                    d="m12.301 0h.093c2.242 0 4.34.613 6.137 1.68l-.055-.031c1.871 1.094 3.386 2.609 4.449 4.422l.031.058c1.04 1.769 1.654 3.896 1.654 6.166 0 5.406-3.483 10-8.327 11.658l-.087.026c-.063.02-.135.031-.209.031-.162 0-.312-.054-.433-.144l.002.001c-.128-.115-.208-.281-.208-.466 0-.005 0-.01 0-.014v.001q0-.048.008-1.226t.008-2.154c.007-.075.011-.161.011-.249 0-.792-.323-1.508-.844-2.025.618-.061 1.176-.163 1.718-.305l-.076.017c.573-.16 1.073-.373 1.537-.642l-.031.017c.508-.28.938-.636 1.292-1.058l.006-.007c.372-.476.663-1.036.84-1.645l.009-.035c.209-.683.329-1.468.329-2.281 0-.045 0-.091-.001-.136v.007c0-.022.001-.047.001-.072 0-1.248-.482-2.383-1.269-3.23l.003.003c.168-.44.265-.948.265-1.479 0-.649-.145-1.263-.404-1.814l.011.026c-.115-.022-.246-.035-.381-.035-.334 0-.649.078-.929.216l.012-.005c-.568.21-1.054.448-1.512.726l.038-.022-.609.384c-.922-.264-1.981-.416-3.075-.416s-2.153.152-3.157.436l.081-.02q-.256-.176-.681-.433c-.373-.214-.814-.421-1.272-.595l-.066-.022c-.293-.154-.64-.244-1.009-.244-.124 0-.246.01-.364.03l.013-.002c-.248.524-.393 1.139-.393 1.788 0 .531.097 1.04.275 1.509l-.01-.029c-.785.844-1.266 1.979-1.266 3.227 0 .025 0 .051.001.076v-.004c-.001.039-.001.084-.001.13 0 .809.12 1.591.344 2.327l-.015-.057c.189.643.476 1.202.85 1.693l-.009-.013c.354.435.782.793 1.267 1.062l.022.011c.432.252.933.465 1.46.614l.046.011c.466.125 1.024.227 1.595.284l.046.004c-.431.428-.718 1-.784 1.638l-.001.012c-.207.101-.448.183-.699.236l-.021.004c-.256.051-.549.08-.85.08-.022 0-.044 0-.066 0h.003c-.394-.008-.756-.136-1.055-.348l.006.004c-.371-.259-.671-.595-.881-.986l-.007-.015c-.198-.336-.459-.614-.768-.827l-.009-.006c-.225-.169-.49-.301-.776-.38l-.016-.004-.32-.048c-.023-.002-.05-.003-.077-.003-.14 0-.273.028-.394.077l.007-.003q-.128.072-.08.184c.039.086.087.16.145.225l-.001-.001c.061.072.13.135.205.19l.003.002.112.08c.283.148.516.354.693.603l.004.006c.191.237.359.505.494.792l.01.024.16.368c.135.402.38.738.7.981l.005.004c.3.234.662.402 1.057.478l.016.002c.33.064.714.104 1.106.112h.007c.045.002.097.002.15.002.261 0 .517-.021.767-.062l-.027.004.368-.064q0 .609.008 1.418t.008.873v.014c0 .185-.08.351-.208.466h-.001c-.119.089-.268.143-.431.143-.075 0-.147-.011-.214-.032l.005.001c-4.929-1.689-8.409-6.283-8.409-11.69 0-2.268.612-4.393 1.681-6.219l-.032.058c1.094-1.871 2.609-3.386 4.422-4.449l.058-.031c1.739-1.034 3.835-1.645 6.073-1.645h.098-.005zm-7.64 17.666q.048-.112-.112-.192-.16-.048-.208.032-.048.112.112.192.144.096.208-.032zm.497.545q.112-.08-.032-.256-.16-.144-.256-.048-.112.08.032.256.159.157.256.047zm.48.72q.144-.112 0-.304-.128-.208-.272-.096-.144.08 0 .288t.272.112zm.672.673q.128-.128-.064-.304-.192-.192-.32-.048-.144.128.064.304.192.192.32.044zm.913.4q.048-.176-.208-.256-.24-.064-.304.112t.208.24q.24.097.304-.096zm1.009.08q0-.208-.272-.176-.256 0-.256.176 0 .208.272.176.256.001.256-.175zm.929-.16q-.032-.176-.288-.144-.256.048-.224.24t.288.128.225-.224z"
                  ></path>
                </g>
              </svg>
              <span class="text-sm font-bold">LinkedIn</span>
            </a>
          </div>
        </div>
      </div>
      <AppForm />
    </section>
  </main>
</template>
