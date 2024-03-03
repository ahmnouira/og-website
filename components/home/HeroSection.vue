<script setup>
import OverviewCards from "../OverviewCards";
import Button from "../Button.vue";
</script>

<template>
  <div
    id="home"
    class="mx-auto p-4 sm:p-6 lg:p-16 w-full 2xl:max-w-[80%] flex flex-col justify-center md:mt-4"
  >
    <div class="flex flex-col justify-center">
      <h1 class="font-bold text-4xl xl:text-5xl text-white">
        Elevate your Trading with OGREEN: Power, Performance, and Efficiency.
      </h1>
      <h3 class="text-white text-2xl my-8">
        Experience the difference with OGREEN. Maximize your potential with our
        high-performance
        <br />
        platform and efficient tools.
      </h3>
      <div class="mt-8">
        <div class="flex space-x-4">
          <Button :text="'Create account'" />
          <Button :text="'Learn more'" :outlined="true" />
        </div>
      </div>
    </div>

    <div class="my-16">
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
        <OverviewCards />
      </div>
    </div>
  </div>
</template>
