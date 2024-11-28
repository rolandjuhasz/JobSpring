<script setup>
import {defineProps} from 'vue';

defineProps({
    title: {
        type: String,
        default: 'Your Next Job Awaits'
    },
    subtitle: {
        type: String,
        default: 'Find the best job that fits your skills and needs'
    }
})
</script>

<template>
    <section class="bg-gray-100 py-20 mb-4">
      <div
        class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col items-center"
      >
        <div class="text-center">
          <h1
            class="text-4xl font-extrabold text-pink-900 sm:text-5xl md:text-6xl"
          >
            {{title}}
          </h1>
          <p class="my-4 text-xl text-black font-bold">
            {{subtitle}}
          </p>
        </div>
      </div>
    </section>
</template>