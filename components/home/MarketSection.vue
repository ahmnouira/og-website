<script setup></script>

<template>
  <div
    id="features"
    class="mx-auto p-4 sm:p-6 lg:p-12 max-w-[80%] w-full flex flex-col justify-center"
  >
    <div class="flex justify-center">
      <h1 class="font-bold text-5xl text-white">
        The Features we have for you
      </h1>
    </div>
    <div class="my-16">
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
        <MarketPerformanceCards />
      </div>
    </div>
  </div>
</template>
