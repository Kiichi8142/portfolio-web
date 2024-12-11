<script setup>
</script>

<template>
  <div>

    <!-- about me -->
    <div class="p-24 max-w-7xl mx-auto">
      <div class="flex-col justify-center space-y-2">
        <div class="flex items-end justify-center space-x-2">
          <p class="text-3xl font-bold">Hi!</p>
          <p class="text-3xl font-bold">I'm Vatchapon</p>
        </div>
        <div>
          <p class="text-norm">I am currently a computer science student from Maejo University, with a foundation in programming and software development, and experienced in machine learning and predictive model.</p>
        </div>
      </div>
    </div>

    <!-- project section -->

    <div class="bg-zinc-900 border-t border-b border-zinc-800">
      <div class="max-w-7xl mx-auto p-24">
        <p class="text-3xl font-bold text-center">A project I've developed during university/academic project</p>

        <!-- tab section -->
        <div class="mt-16">
          <div class="space-x-4">
            <button class="proj-btn-active">AAC</button>
            <button class="proj-btn-inactive">ESO</button>
          </div>
          <div class="mt-4 grid grid-cols-1 lg:grid-cols-2">
            <div class="space-y-2">
              <p class="font-semibold text-sky-400">Frontend</p>
              <p class="text-xl">Another Anime Collection</p>
              <p class="text-lg text-zinc-400">A basic anime progress tracking website that allows you to bookmark your anime and be able to update your bookmark status, episodes watched, and score your anime.</p>
            </div>
          </div>
          <div class="h-[40rem] max-w-7xl w-full absolute mt-8">
            <div class="lg:absolute -left-10 lg:w-[38rem] w-full lg:h-[28rem] proj-img-prev">
              <img class="object-cover w-full h-full rounded-md" src="/src/assets/images/aac-1.png" alt="">
            </div>
            <div class="lg:absolute lg:right-5 lg:top-5 w-full lg:w-[42rem] lg:h-[20rem] proj-img-prev">
              <img class="object-cover w-full h-full rounded-md" src="/src/assets/images/aac-2.png" alt="">
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- skills section -->

    <div class="bg-zinc-900 border-t border-b border-zinc-800 mt-[40rem]">
      <div class="p-24 max-w-7xl mx-auto space-y-2">
        <p class="text-3xl font-bold text-center mb-16">Skills</p>
        <div class="flex justify-center">
          <i class="devicon-vuejs-line-wordmark"></i>
        </div>

        <div class="space-y-4">
          <div class="space-y-0.5">
            <p class="text-lg text-green-400">Technical Skills</p>
            <p class="text-xl">Vue.js, Laravel, Javascript, TailwindCSS, Python, Tensorflow, Colab, Lua, C#</p>
          </div>
          <div class="space-y-0.5">
            <p class="text-lg text-green-400">Soft Skills</p>
            <p class="text-xl">Problem-solving, Flexibility, Open-Mindedness</p>
          </div>
        </div>

      </div>
    </div>

  </div>
</template>

<style scoped>

.text-norm {
  @apply text-xl text-zinc-200 text-center
}

.proj-btn-active {
  @apply py-4 px-6 text-lg font-semibold bg-zinc-50 text-zinc-950 rounded-md
}

.proj-btn-inactive {
  @apply py-4 px-6 text-lg font-semibold border border-zinc-800 rounded-md
}

.proj-btn-inactive:hover {
  @apply bg-zinc-800
}

.proj-img-prev {
  @apply border border-zinc-800 rounded-md shadow-md
}

</style>
