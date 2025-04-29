<template>
    <Disclosure as="nav" v-slot="{ open } " style="background: #302C42;">
        <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8 mt-2">
            <div class="relative flex h-16 items-center justify-between">
                <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
                    <!-- Mobile menu button-->
                    <DisclosureButton
                        class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-700 hover:text-white focus:ring-2 focus:ring-white focus:outline-hidden focus:ring-inset">
                        <span class="absolute -inset-0.5" />
                        <span class="sr-only">Open main menu</span>
                        <Bars3Icon v-if="!open" class="block size-6" aria-hidden="true" />
                        <XMarkIcon v-else class="block size-6" aria-hidden="true" />
                    </DisclosureButton>
                </div>
                <div class="flex items-center justify-center sm:items-stretch sm:justify-start">
                    <div class="flex shrink-0 items-center sm:ml-0">
                        <img class="h-14 w-auto" src="~assets/logo.png" alt="Your Company" />
                    </div>
                </div>
                <div class="hidden sm:ml-6 sm:block">
                    <div class="flex justify-center space-x-4 font-montserrat">
                        <a v-for="item in navigation" :key="item.name" :href="item.href"
                            :class="[item.current ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']"
                            :aria-current="item.current ? 'page' : undefined">{{ item.name }}</a>
                    </div>
                </div>
                <div
                    class="absolute inset-y-0 right-0 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0 space-x-2">
                    <!-- Outlined button -->
                    <button type="button"
                        class="relative rounded-md border border-white px-4 py-1.5 text-sm font-medium text-white hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800 transition-colors duration-200">
                        CONTACT US
                    </button>

                    <!-- Gradient button -->
                    <button type="button"
                        class="relative rounded-md px-4 py-1.5 text-sm font-medium text-white focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-gray-800 bg-gradient-to-r from-gray-800 to-purple-600 hover:from-blue-600 hover:to-purple-700 transition-all duration-200">
                        JOIN HYDRA
                    </button>
                </div>
            </div>
        </div>

        <DisclosurePanel class="sm:hidden">
            <div class="space-y-1 px-2 pt-2 pb-3">
                <DisclosureButton v-for="item in navigation" :key="item.name" as="a" :href="item.href"
                    :class="[item.current ? 'bg-gray-900 text-white' : 'text-gray-300 hover:bg-gray-700 hover:text-white', 'block rounded-md px-3 py-2 text-base font-medium']"
                    :aria-current="item.current ? 'page' : undefined">{{ item.name }}</DisclosureButton>
                <div class="flex space-x-2 pt-2">
                    <button type="button"
                        class="w-full rounded-md border border-white px-4 py-2 text-base font-medium text-white hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-white">
                        CONTACT US
                    </button>
                    <button type="button"
                        class="w-full rounded-md px-4 py-2 text-base font-medium text-white bg-gradient-to-r from-blue-500 to-purple-600 hover:from-blue-600 hover:to-purple-700">
                        JOIN HYDRA
                    </button>
                </div>
            </div>
        </DisclosurePanel>
    </Disclosure>
</template>

<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel, Menu, MenuButton, MenuItem, MenuItems } from '@headlessui/vue'
import { Bars3Icon, BellIcon, XMarkIcon } from '@heroicons/vue/24/outline'

const navigation = [
    { name: 'ABOUT', href: '#', current: true },
    { name: 'SERVICES', href: '#', current: false },
    { name: 'TECHNOLOGIES', href: '#', current: false },
    { name: 'HOW TO', href: '#', current: false },
]
</script>

<style scoped>
/* Add any custom styles here if needed */
</style>