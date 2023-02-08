<template>
    <div class="min-h-screen bg-gray-100">
      <Popover as="template" v-slot="{ open }">
        <header :class="[open ? 'fixed inset-0 z-40 overflow-y-auto' : '', 'bg-white shadow-sm lg:static lg:overflow-y-visible']">
          <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
            <div class="relative flex justify-between lg:gap-8 xl:grid xl:grid-cols-12">
              <div class="min-w-0 flex-1 md:px-8 lg:px-0 xl:col-span-6">
                <div class="flex items-center px-6 py-4 md:mx-auto md:max-w-3xl lg:mx-0 lg:max-w-none xl:px-0">
                  <div class="w-full">
                    <label for="search" class="sr-only">Search</label>
                    <div class="relative">
                      <div class="pointer-events-none absolute inset-y-0 left-0 flex items-center pl-3">
                        <MagnifyingGlassIcon class="h-5 w-5 text-gray-400" aria-hidden="true" />
                      </div>
                      <input id="search" name="search" class="block w-full rounded-md border border-gray-300 bg-white py-2 pl-10 pr-3 text-sm placeholder-gray-500 focus:border-indigo-500 focus:text-gray-900 focus:placeholder-gray-400 focus:outline-none focus:ring-1 focus:ring-indigo-500 sm:text-sm" placeholder="Search" type="search" />
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </header>
      </Popover>
  
      <div class="shown py-6 outline outline-1 outline-gray-400">
        <div class="mx-auto max-w-6xl grid max-w-8xl grid-cols-12 gap-7 px-8">
          <div class="col-span-4">
            <div class="sticky top-6 divide-y divide-gray-300">
              <!-- Your content -->
              <ul class="border-dashed border-2 border-gray-300 rounded-2xl py-2 px-3">
                <li>aaa</li>
                <li>bbb</li>
                <li>ccc</li>
              </ul>
            </div>
          </div>
          <div class="col-span-8">
            <!-- Your content -->
            <ul class="border-dashed border-2 border-red-300 rounded-2xl  py-2 px-3">
                <li>aaa</li>
                <li>bbb</li>
                <li>ccc</li>
              </ul>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  import { Popover, PopoverButton, PopoverPanel } from '@headlessui/vue'
  import { MagnifyingGlassIcon } from '@heroicons/vue/20/solid'
  import { Bars3Icon, BellIcon, XMarkIcon } from '@heroicons/vue/24/outline'
  
  const user = {
    name: 'Chelsea Hagon',
    email: 'chelsea.hagon@example.com',
    imageUrl:
      'https://images.unsplash.com/photo-1550525811-e5869dd03032?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80',
  }
  const languageKeys = [
    { key: 'finance',  value: '金融' },
    { key: 'exchange',  value: '幣幣' },
    { key: 'selfmarket',  value:'自選' },
    { key: 'allmarket',  value: '全部行情' },
  ]
  const userNavigation = [
    { name: 'Your Profile', href: '#' },
    { name: 'Settings', href: '#' },
    { name: 'Sign out', href: '#' },
  ]
  </script>