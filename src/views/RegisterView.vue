<template>
  <div class="min-h-screen flex items-center justify-center bg-blue-50">
    <div class="bg-white rounded-lg shadow-lg p-8 max-w-sm w-full">
      <h1 class="text-2xl font-bold text-gray-500 text-center mb-6">Register</h1>
      <form>
        <div class="mb-4">
          <label for="name" class="block text-gray-500 font-medium mb-2">Full Name</label>
          <input
            type="text"
            id="name"
            class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-600"
            placeholder="Enter your full name"
            required
          />
        </div>

        <div class="mb-4">
          <label for="email" class="block text-gray-500 font-medium mb-2">Email</label>
          <input
            type="email"
            id="email"
            class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-600"
            placeholder="Enter your email"
            required
          />
        </div>

        <div class="mb-4">
          <label for="password" class="block text-gray-500 font-medium mb-2">Password</label>
          <input
            type="password"
            id="password"
            class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-600"
            placeholder="Enter your password"
            required
          />
        </div>

        <div class="mb-6">
          <label for="confirm-password" class="block text-gray-500 font-medium mb-2">Confirm Password</label>
          <input
            type="password"
            id="confirm-password"
            class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-600"
            placeholder="Confirm your password"
            required
          />
        </div>

        <div class="mb-6">
          <label for="registration-type" class="block text-gray-500 font-medium mb-2">How are you registering?</label>
          <select
            id="registration-type"
            class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-600"
            required
          >
            <option value="">Select an option</option>
            <option value="job-seeker">As a Job Seeker</option>
            <option value="company">As a Company</option>
          </select>
        </div>

        <button
          type="submit"
          class="w-full bg-pink-900 text-white py-3 rounded-lg font-semibold hover:bg-pink-700 transition"
        >
          Register
        </button>
      </form>
    </div>
  </div>
</template>