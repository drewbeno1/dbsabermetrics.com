<script setup>
  import MainLayout from '../layouts/MainLayout.vue';
  import Footer from '../components/Footer.vue';
</script>

<template>
  <MainLayout>
      <div class="py-24 sm:py-32 lg:pb-40">
        <div class="mx-auto max-w-7xl px-6 lg:px-8">
          <div class="mx-auto max-w-2xl text-center">
            <h1 class="text-4xl font-bold tracking-tight text-white sm:text-6xl">Player Development Redefined</h1>
            <p class="mt-6 text-lg leading-8 text-gray-300">DataBase Sabermetrics delivers the intuitive pitch-tracking software and advanced analytics needed to bring your team to the next level. Get in the game, click below to get started!</p>
            <div class="mt-10 flex items-center justify-center gap-x-6">
              <a href="/contact/" class="rounded-md bg-indigo-500 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-400 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-400">Get started</a>
              <a href="/product/" class="text-sm font-semibold leading-6 text-white">Learn more <span aria-hidden="true">→</span></a>
            </div>
          </div>
          <img src="../assets/DashboardScreenshot.png" alt="App screenshot" width="2432" height="1442" class=" opacity-95 mt-16 rounded-md bg-white/5 shadow-2xl ring-1 ring-white/10 sm:mt-24" />
        </div>
      </div>
      <div class="absolute inset-x-0 top-[calc(100%-13rem)] -z-10 transform-gpu overflow-hidden blur-3xl sm:top-[calc(100%-30rem)]" aria-hidden="true">
        <div class="relative left-[calc(50%+3rem)] aspect-[1155/678] w-[36.125rem] -translate-x-1/2 bg-gradient-to-tr from-[#ff80b5] to-[#9089fc] opacity-20 sm:left-[calc(50%+36rem)] sm:w-[72.1875rem]" style="clip-path: polygon(74.1% 44.1%, 100% 61.6%, 97.5% 26.9%, 85.5% 0.1%, 80.7% 2%, 72.5% 32.5%, 60.2% 62.4%, 52.4% 68.1%, 47.5% 58.3%, 45.2% 34.5%, 27.5% 76.7%, 0.1% 64.9%, 17.9% 100%, 27.6% 76.8%, 76.1% 97.7%, 74.1% 44.1%)" />
      </div>
  </MainLayout>
  <Footer />
</template>