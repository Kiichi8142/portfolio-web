<script setup>
import { DevicePhoneMobileIcon, EnvelopeIcon, GlobeAltIcon, UserIcon } from '@heroicons/vue/16/solid';
import { ref } from 'vue';

const activeTab = ref(1)

const setTab = (tab) => {
  activeTab.value = tab
}

</script>

<template>
  <div>

    <header class="p-4 border-b border-zinc-800 sticky top-0 z-50 backdrop-blur-md">
      <div class="flex justify-end space-x-8 font-semibold max-w-7xl mx-auto">
        <a href="#home">Home</a>
        <a href="#project">Project</a>
        <a href="#skills">Skills</a>
        <a href="#experience">Experience</a>
        <a href="#contact">Contact</a>
      </div>
    </header>

    <!-- about me -->
    <div id="home" class="p-8 lg:p-24 max-w-7xl mx-auto my-32">
      <div class="flex-col justify-center space-y-2">
        <div class="flex items-end justify-center space-x-2">
          <p class="text-3xl font-bold">Hi!</p>
          <p class="text-3xl font-bold">I'm Vatchapon</p>
        </div>
        <div class="space-y-4">
          <p class="text-norm">I am currently a computer science student from Maejo University, with a foundation in programming and software development, and experienced in machine learning and predictive model.</p>
          <p class="text-norm">I am seeking opportunities to apply and expand my skills in a 
            challenging internship and further develop expertise in the field.</p>
        </div>
      </div>
    </div>

    <!-- project section -->

    <div id="project" class="bg-zinc-900 border-t border-b border-zinc-800">
      <div class="max-w-7xl mx-auto p-8 lg:p-24">
        <p class="text-3xl font-bold text-center">A project I've developed during university/academic project</p>

        <!-- tab section -->
        <div class="mt-16">
          <div class="space-x-4">
            <button @click="setTab(1)" :class="{'proj-btn-active': activeTab === 1, 'proj-btn-inactive': activeTab !== 1}">AAC</button>
            <button @click="setTab(2)" :class="{'proj-btn-active': activeTab === 2, 'proj-btn-inactive': activeTab !== 2}">ESO</button>
          </div>
          
          <!-- Tab 1 -->
          <div v-if="activeTab === 1" class="mt-4 grid grid-cols-1 lg:grid-cols-2 space-y-2">
            <div class="space-y-2">
              <p class="font-semibold text-sky-400">Frontend</p>
              <p class="text-xl">Another Anime Collection</p>
              <p class="text-lg text-zinc-400">A basic anime progress tracking website that allows you to bookmark your anime and be able to update your bookmark status, episodes watched, and score your anime.</p>
            </div>
            <div class="space-y-2 py-4 lg:py-0">
              <img class="mx-auto" src="https://skillicons.dev/icons?i=js,html,css,tailwind,vue" alt="">
            </div>
          </div>
          <div v-if="activeTab === 1" class="absolute left-1/2 transform -translate-x-1/2 max-w-2xl lg:max-w-7xl w-full mx-auto my-10">
            <div class="lg:space-x-4 space-y-2 lg:space-y-0 lg:flex">
              <img class="object-cover w-full h-full lg:w-[40rem] rounded-md proj-img-prev" src="/src/assets/images/aac-1.png" alt="">
              <img class="object-cover w-full h-full lg:w-[40rem] rounded-md proj-img-prev lg:self-center" src="/src/assets/images/aac-2.png" alt="">
            </div>
          </div>

          <!-- Tab 2 -->
          <div v-if="activeTab === 2" class="mt-4 grid grid-cols-1 lg:grid-cols-2 space-y-2">
            <div class="space-y-2">
              <p class="font-semibold text-sky-400">Fullstack</p>
              <p class="text-xl">Evaluation System for Organization</p>
              <p class="text-lg text-zinc-400">A system designed for organizations where both employers and employees can evaluate themselves. In a team-based structure, team members assess their own performance, while the team leader evaluates all team members, including themselves.</p>
            </div>
            <div class="space-y-2 py-4 lg:py-0">
              <img class="mx-auto" src="https://skillicons.dev/icons?i=laravel,php,js,html,css,tailwind,vue" alt="">
            </div>
          </div>
          <div v-if="activeTab === 2" class="absolute left-1/2 transform -translate-x-1/2 max-w-2xl lg:max-w-7xl w-full mx-auto my-10">
            <div class="lg:space-x-4 space-y-2 lg:space-y-0 lg:flex">
              <img class="object-cover w-full h-full lg:w-[40rem] rounded-md proj-img-prev" src="/src/assets/images/eso-1.png" alt="">
              <img class="object-cover w-full h-full lg:w-[40rem] rounded-md proj-img-prev lg:self-center" src="/src/assets/images/eso-2.png" alt="">
            </div>
          </div>

        </div>
      </div>
    </div>

    <!-- skills section -->

    <div id="skills" class="bg-zinc-900 border-t border-b border-zinc-800 mt-[55rem] lg:mt-[42rem]">
      <div class="p-8 lg:p-24 max-w-7xl mx-auto space-y-2">
        <div class="flex-col justify-center items-center space-y-2 mb-16">
          <p class="text-3xl font-bold text-center">Skills</p>
          <img class="mx-auto" src="https://skillicons.dev/icons?i=js,html,css,tailwind,cs,unity,py,tensorflow,kotlin,laravel,lua,mongodb,mysql,php,pinia,vue,vscode,c" alt="">
        </div>

        <div class="space-y-8">
          <div class="space-y-2">
            <p class="text-green-400">Technical Skills</p>
            <div class="skills-grid">
              <p class="text-lg font-semibold">Framework</p>
              <p class="text-lg text-zinc-400">Laravel, Vue.js, TailwindCSS, Tensorflow, Unity</p>
            </div>
            <div class="skills-grid">
              <p class="text-lg font-semibold">Computer Languages</p>
              <p class="text-lg text-zinc-400">Javascript, Python, Colab, Lua, C#, C++, Kotlin, PHP, SQL</p>
            </div>
            <div class="skills-grid">
              <p class="text-lg font-semibold">Databases</p>
              <p class="text-lg text-zinc-400">MongoDB, MySQL, MariaDB</p>
            </div>
          </div>
          <div class="space-y-2">
            <p class="text-green-400">Soft Skills</p>
            <p class="text-xl">Problem-solving, Flexibility, Open-Mindedness</p>
          </div>
          <div class="space-y-2">
            <p class="text-green-400">Languages</p>
            <p class="text-xl">Thai, English</p>
          </div>
        </div>

      </div>
    </div>

    <!-- Education/Experience section -->

    <div id="experience" class="">
      <div class="p-8 lg:p-24 max-w-7xl mx-auto space-y-2">
        <div class="flex-col justify-center items-center space-y-2 py-2">
          <p class="text-xl text-sky-600">Educations</p>
        </div>

        <div class="space-y-4">
          <div class="grid grid-cols-2">
            <div class="space-y-0.5">
              <p class="text-xl font-semibold">Vocational Certificate Information Technology</p>
              <p class="text-lg text-zinc-600">Lanna Polytechnic ChiangMai Technological College</p>
            </div>
            <div class="flex flex-col items-end space-y-0.5">
              <p class="text-xl font-semibold">Chiang Mai, Thailand</p>
              <p class="text-lg text-zinc-400">March, 2019</p>
            </div>
          </div>
          <div class="grid grid-cols-2">
            <div class="space-y-0.5">
              <p class="text-xl font-semibold">Bachelor of Science in Computer Science</p>
              <p class="text-lg text-zinc-600">Maejo University</p>
            </div>
            <div class="flex flex-col items-end space-y-0.5">
              <p class="text-xl font-semibold">Chiang Mai, Thailand</p>
              <p class="text-lg text-zinc-400">March, 2026</p>
            </div>
          </div>
        </div>

        <div class="pt-10">
        </div>
        <div class="space-y-2">
          <p class="text-xl text-sky-600">Work Experience</p>
          <p class="text-2xl font-bold">Internship at Data Academy</p>
          <p class="text-lg text-zinc-200">I was sent to work as an intern at the ICT Center at Dara Academy. Most of the work was solving any problems their employee had. For example, printer gets stuck, collects/updates computer information, sets up LAN cable or router, and helps set up places for events.</p>
          <p class="text-lg text-zinc-200">I've learned a lot about work cultures there and, most importantly, Christian religion, which is the main religion at Dara Academy.</p>
          <p class="text-lg text-zinc-200"></p>
        </div>

      </div>
    </div>

    <!-- contacts section -->

    <div id="contact" class="bg-zinc-900 border-t border-b border-zinc-800">
      <div class="p-16 max-w-7xl mx-auto space-y-2">
        <div class="flex-col justify-center items-center space-y-4">
          <p class="text-3xl font-bold text-center">Contacts</p>
          <div class="grid grid-cols-3 text-zinc-200 place-items-center">

            <div>
              <div class="flex items-center space-x-2">
                <UserIcon class="size-5" />
                <p class="text-lg">Vatchapon Ponsuwan</p>
              </div>
              <div class="flex items-center space-x-2">
                <DevicePhoneMobileIcon class="size-5" />
                <p class="text-lg">090-320-9968</p>
              </div>
            </div>

            <div>
              <div class="flex items-center space-x-2">
                <GlobeAltIcon class="size-5" />
                <p class="text-lg">ChiangMai, Thailand</p>
              </div>
              <div class="flex items-center space-x-2">
                <EnvelopeIcon class="size-5" />
                <p class="text-lg">vponsuwan@gmail.com</p>
              </div>
            </div>

            <div>
              <a href="https://github.com/Kiichi8142" target="_blank" class="flex items-center space-x-2">
                <img class="mx-auto size-5" src="https://skillicons.dev/icons?i=github" alt="">
                <p class="text-lg">Kiichi8142</p>
              </a>
              <a href="https://www.linkedin.com/in/vatchapon-ponsuwan-90957a341/" target="_blank" class="flex items-center space-x-2">
                <img class="mx-auto size-5" src="https://skillicons.dev/icons?i=linkedin" alt="">
                <p class="text-lg">Linkedin</p>
              </a>
            </div>

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

.skills-grid {
  @apply grid grid-cols-2
}

</style>
