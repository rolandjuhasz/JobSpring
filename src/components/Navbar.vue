<script setup>
    import logo from '@/assets/img/logo-bg.png'
    import { RouterLink, useRoute } from 'vue-router';

    const isActiveLink = (routepath) => {
      const route = useRoute();
      return route.path === routepath;
    }
</script>

<template>
    <nav class="bg-pink-900 border-b">
      <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
        <div class="flex h-20 items-center justify-between">
          <a href="/"><img class="h-20 w-auto" :src="logo" alt="Vue Jobs"/></a>
          <div
            class="flex flex-1 items-center justify-center md:items-stretch md:justify-start"
            >
            <!-- Logo -->
            <RouterLink class="flex flex-shrink-0 items-center mr-4" to="/">
              <span class="hidden md:block text-white text-2xl font-bold ml-2"
              >JobSpring</span
              >
            </RouterLink>
            <div class="md:ml-auto">
              <div class="flex space-x-2">
                <RouterLink
                  to="/"
                  :class="[isActiveLink('/')  ? 'text-orange-400' : 'hover:text-gray-900 hover:text-white', 'text-white', 'px-3', 'py-2', 'rounded-md']"
                  >Home</RouterLink>
                  <RouterLink
                  to="/jobs"
                  :class="[isActiveLink('/jobs')  ? 'text-orange-400' : 'hover:text-gray-900 hover:text-white', 'text-white', 'px-3', 'py-2', 'rounded-md']"
                  >Jobs</RouterLink>
                  <RouterLink
                  to="/jobs/add"
                  :class="[isActiveLink('/jobs/add')  ? 'text-orange-400' : 'hover:text-gray-900 hover:text-white', 'text-white', 'px-3', 'py-2', 'rounded-md']"
                  >Add jobs</RouterLink>
                  <RouterLink
                  to="/register"
                  :class="[isActiveLink('/register')  ? 'text-orange-400' : 'hover:text-gray-900 hover:text-white', 'text-white', 'px-3', 'py-2', 'rounded-md']"
                  >Register</RouterLink>
                  <RouterLink
                  to="/login"
                  :class="[isActiveLink('/login')  ? 'text-orange-400' : 'hover:text-gray-900 hover:text-white', 'text-white', 'px-3', 'py-2', 'rounded-md']"
                  >Loign</RouterLink>
              </div>
            </div>
          </div>
        </div>
      </div>
    </nav>

    </template>