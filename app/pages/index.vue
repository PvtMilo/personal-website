<template>
  <main class="flex flex-col items-center">
    <section
      class="w-full lg:max-w-7xl lg:min-h-[calc(100dvh-5rem)] flex flex-col justify-center border-b-2 border-white"
    >
      <div
        class="grid lg:grid-cols-4 lg:grid-rows-4 place-items-center lg:place-items-start gap-4 lg:gap-2 text-center text-white"
      >
        <h1
          class="lg:col-start-1 lg:col-end-4 border-2 text-3xl lg:text-7xl font-semibold"
        >
          ILHAM DWI PAMBUDI
        </h1>
        <h2 class="lg:col-start-1 lg:col-end-4 border-2 text-2xl lg:text-6xl">
          Full-Stack Developer
        </h2>

        <div
          class="lg:col-start-4 lg:row-start-1 lg:row-end-5 lg:place-self-center border-2 h-50 w-50 xl:h-70 xl:w-70 rounded-full overflow-hidden"
        >
          <NuxtImg class="h-full w-full object-cover" src="/avatar.jpg" />
        </div>

        <p
          class="lg:col-start-1 lg:col-end-4 border-2 lg:text-xl lg:text-left lg:max-w-2xl"
        >
          A passionate web developer focused on building modern and meaningful
          digital experiences.
        </p>
        <button class="lg:row-start-4 border-2 rounded-xl px-4 py-2">
          Learn More
        </button>
      </div>
    </section>
    <section class="h-screen">
      <h2>Tech Stack</h2>
    </section>
    <section>
      <h2>Works</h2>
    </section>
    <section>
      <h2>Journey</h2>
    </section>
    <section>
      <h2>Contact</h2>
    </section>
  </main>
</template>
