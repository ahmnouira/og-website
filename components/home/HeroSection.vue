<script setup>
import OverviewCards from "../OverviewCards";
import Button from "../Button.vue";
</script>

<template>
  <div
    id="home"
    class="mx-auto p-4 sm:p-6 lg:p-12 max-w-[80%] w-full h-[80vh] flex flex-col justify-center"
  >
    <h1 class="font-bold text-5xl text-white">
      The next generation high-performance algotrading platform
    </h1>
    <h3 class="text-white text-2xl my-8">
      The most powerful strategy using Python and Cython with the raw speed of C
      <br />
      To create the ultimate algotrading experience.
    </h3>
    <div class="mt-8 mb-16">
      <div class="flex space-x-4">
        <Button :text="'Create account'" />
        <Button :text="'Learn more'" :outlined="true" />
      </div>
    </div>
    <div class="my-8">
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
        <OverviewCards />
      </div>
    </div>
  </div>
</template>
