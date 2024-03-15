<template>
    <div class="bg-gray-200 min-h-screen flex flex-col items-center justify-center">
    <div class="w-full max-w-lg mb-10">
      <input
        placeholder="(Search)"
        class="w-full p-1 text-base border-2 border-gray-500 rounded-md focus:outline-none focus:ring-2 focus:ring-gray-400"
        style="line-height: 1.5rem; text-align: center;"
      />
    </div>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-16 px-7 w-full max-w-3xl">
      <div v-for="index in 4" :key="index" class="bg-gray-300 shadow rounded-2xl overflow-hidden">
        <div class="relative pt-6 pb-4 px-6">
          <div class="absolute inset-0 flex items-center justify-center">
            <span class="text-gray-500 text-sm">(Picture)</span>
          </div>
          <div class="w-full bg-gray-100 h-24 rounded-md"></div>
        </div>
        <div class="px-5 pb-2">
          <div class="flex items-center">
            <div class="bg-gray-400 rounded-full h-12 w-12"></div>
            <div class="flex-1 ml-9 space-y-3">
              <div class="h-1 bg-gray-400 rounded w-5/5"></div>
              <div class="h-1 bg-gray-400 rounded w-5/5"></div>
              <div class="h-1 bg-gray-400 rounded w-5/5"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
// No logic for this component yet
</script>

<style scoped>
/* Placeholder color */
input::placeholder {
  color: #718096; /* Use gray-500 */
}
</style>