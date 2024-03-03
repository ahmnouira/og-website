<script setup>
const props = defineProps({
  title: { type: String, required: true },
  description: { type: String, required: true },
  value: { type: String, required: true },
});
</script>

<template>
  <div class="flex dark:bg-zinc-900">
    <div class="flex flex-col w-full">
      <div class="border-b-4 border-orange-700">
        <h2 class="text-2xl font-semibold m-4 text-white">{{ props.title }}</h2>
      </div>
      <p class="text-gray-700 m-4">{{ props.description }}</p>
    </div>
    <div
      class="flex items-end border-l-4 border-orange-700 p-2 md:min-w-32 md:overflow-hidden md:justify-center"
    >
      <h3 class="text-3xl font-bold text-green-700">{{ props.value }}</h3>
    </div>
  </div>
</template>
