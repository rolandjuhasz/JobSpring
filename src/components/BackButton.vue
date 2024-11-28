<script setup>
import { RouterLink } from 'vue-router';

</script>

<template>
       <section>
      <div class="container m-auto py-6 px-6">
        <RouterLink
          to="/jobs"
          class="text-pink-900 hover:text-pink-600 flex items-center"
        >
          <i class="fas fa-arrow-left mr-2"></i> Back to Job Listings
        </RouterLink>
      </div>
    </section>
</template>