<script setup>
import MainLayout from '../layouts/MainLayout.vue';
const posts = [
//   {
//     id: 1,
//     title: 'Boost your conversion rate',
//     href: '#',
//     description:
//       'Illo sint voluptas. Error voluptates culpa eligendi. Hic vel totam vitae illo. Non aliquid explicabo necessitatibus unde. Sed exercitationem placeat consectetur nulla deserunt vel. Iusto corrupti dicta.',
//     date: 'Mar 16, 2020',
//     datetime: '2020-03-16',
//     category: { title: 'Marketing', href: '#' },
//     author: {
//       name: 'Michael Foster',
//       role: 'Co-Founder / CTO',
//       href: '#',
//       imageUrl:
//         'https://images.unsplash.com/photo-1519244703995-f4e0f30006d5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80',
//     },
//   },
]
</script>

<template>
    <MainLayout>
        <div class="py-24 sm:py-32">
        <div class="mx-auto max-w-7xl px-6 lg:px-8">
            <div class="mx-auto max-w-2xl lg:mx-0">
            <h2 class="text-base font-semibold leading-7 text-indigo-400">Coming Soon!</h2>
            <h2 class="text-3xl font-bold tracking-tight text-white sm:text-4xl">dataBase Blog</h2>
            <p class="mt-2 text-lg leading-8 text-gray-100">Our blog will discuss all things Sabermetrics across all levels of baseball. Keep an eye out on our social media for updates!</p>
            </div>
            <div class="mx-auto mt-10 grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 border-t border-gray-200 pt-10 sm:mt-16 sm:pt-16 lg:mx-0 lg:max-w-none lg:grid-cols-3">
            <article v-for="post in posts" :key="post.id" class="flex max-w-xl flex-col items-start justify-between">
                <div class="flex items-center gap-x-4 text-xs">
                <time :datetime="post.datetime" class="text-gray-300">{{ post.date }}</time>
                <a :href="post.category.href" class="relative z-10 rounded-full bg-gray-50 px-3 py-1.5 font-medium text-gray-200 hover:bg-gray-100">{{ post.category.title }}</a>
                </div>
                <div class="group relative">
                <h3 class="mt-3 text-lg font-semibold leading-6 text-gray-300 group-hover:text-gray-200">
                    <a :href="post.href">
                    <span class="absolute inset-0" />
                    {{ post.title }}
                    </a>
                </h3>
                <p class="mt-5 line-clamp-3 text-sm leading-6 text-gray-200">{{ post.description }}</p>
                </div>
                <div class="relative mt-8 flex items-center gap-x-4">
                <img :src="post.author.imageUrl" alt="" class="h-10 w-10 rounded-full bg-gray-50" />
                <div class="text-sm leading-6">
                    <p class="font-semibold text-gray-300">
                    <a :href="post.author.href">
                        <span class="absolute inset-0" />
                        {{ post.author.name }}
                    </a>
                    </p>
                    <p class="text-gray-200">{{ post.author.role }}</p>
                </div>
                </div>
            </article>
            </div>
        </div>
        </div>
    </MainLayout>
  </template>