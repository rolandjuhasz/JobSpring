


<template>
    <div class="min-h-screen flex items-center justify-center bg-green-50">
      <div class="bg-white rounded-lg shadow-lg p-8 max-w-sm w-full">
        <h1 class="text-2xl font-bold text-gray-500 text-center mb-6">Login</h1>
        <form>
          <div class="mb-4">
            <label for="email" class="block text-gray-500 font-medium mb-2">Email</label>
            <input
              type="email"
              id="email"
              class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-pink-600"
              placeholder="Enter your email"
              required
            />
          </div>
          <div class="mb-6">
            <label for="password" class="block text-gray-500 font-medium mb-2">Password</label>
            <input
              type="password"
              id="password"
              class="w-full p-3 border rounded-lg focus:outline-none focus:ring-2 focus:ring-pink-600"
              placeholder="Enter your password"
              required
            />
          </div>
          <button
            type="submit"
            class="w-full bg-pink-900 text-white py-3 rounded-lg font-semibold hover:bg-pink-700 transition"
          >
            Login
          </button>
        </form>
      </div>
    </div>
  </template>