<script setup>
import { ChevronDownIcon } from '@heroicons/vue/20/solid'
import MainLayout from '../layouts/MainLayout.vue';
</script>

<template>
    <MainLayout>
        <div class="isolate px-6 py-24 sm:py-32 lg:px-8">
        <div class="mx-auto max-w-2xl text-center">
            <h2 class="text-3xl font-bold tracking-tight text-gray-300 sm:text-4xl">Contact sales</h2>
            <p class="mt-2 text-lg leading-8 text-gray-300">Aute magna irure deserunt veniam aliqua magna enim voluptate.</p>
        </div>
        <form action="#" method="POST" class="mx-auto mt-16 max-w-xl sm:mt-20" netlify>
            <div class="grid grid-cols-1 gap-x-8 gap-y-6 sm:grid-cols-2">
            <div>
                <label for="first-name" class="block text-sm font-semibold leading-6 text-gray-300">First name</label>
                <div class="mt-2.5">
                <input type="text" name="first-name" id="first-name" autocomplete="given-name" class="block w-full bg-gray-200/50 rounded-md border-0 px-3.5 py-2 text-gray-300 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-900 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6" />
                </div>
            </div>
            <div>
                <label for="last-name" class="block text-sm font-semibold leading-6 text-gray-300">Last name</label>
                <div class="mt-2.5">
                <input type="text" name="last-name" id="last-name" autocomplete="family-name" class="block bg-gray-200/50 w-full rounded-md border-0 px-3.5 py-2 text-gray-300 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-900 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6" />
                </div>
            </div>
            <div class="sm:col-span-2">
                <label for="company" class="block text-sm font-semibold leading-6 text-gray-300">Team</label>
                <div class="mt-2.5">
                <input type="text" name="company" id="company" autocomplete="organization" class="block bg-gray-200/50 w-full rounded-md border-0 px-3.5 py-2 text-gray-300 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-900 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6" />
                </div>
            </div>
            <div class="sm:col-span-2">
                <label for="email" class="block text-sm font-semibold leading-6 text-gray-300">Email</label>
                <div class="mt-2.5">
                <input type="email" name="email" id="email" autocomplete="email" class="block bg-gray-200/50 w-full rounded-md border-0 px-3.5 py-2 text-gray-300 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-900 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6" />
                </div>
            </div>
            <div class="sm:col-span-2">
                <label for="phone-number" class="block text-sm font-semibold leading-6 text-gray-300">Phone number</label>
                <div class="relative mt-2.5">
                <div class="absolute inset-y-0 left-0 flex items-center ">
                    <label for="country" class="sr-only">Country</label>
                    <select id="country" name="country" class="h-full rounded-md border-0 bg-none py-0 pl-4 pr-9 text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm">
                    <option>US</option>
                    <option>CA</option>
                    <option>EU</option>
                    </select>
                    <ChevronDownIcon class="pointer-events-none absolute right-3 top-0 h-full w-5 text-gray-400" aria-hidden="true" />
                </div>
                <input type="tel" name="phone-number" id="phone-number" autocomplete="tel" class="block bg-gray-200/50 w-full rounded-md border-0 px-3.5 py-2 pl-20 text-gray-300 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-900 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6" />
                </div>
            </div>
            <div class="sm:col-span-2">
                <label for="message" class="block text-sm font-semibold leading-6 text-gray-300">Message</label>
                <div class="mt-2.5">
                <textarea name="message" id="message" rows="4" class="block bg-gray-200/50 w-full rounded-md border-0 px-3.5 py-2 text-gray-300 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-900 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6" />
                </div>
            </div>
            </div>
            <div class="mt-10">
            <button type="submit" class="block w-full rounded-md bg-indigo-600 px-3.5 py-2.5 text-center text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Let's talk</button>
            </div>
        </form>
        </div>
    </MainLayout>
  </template>