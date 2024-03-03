<script setup>
const props = defineProps({
  title: { type: String, required: true },
  description: { type: String, required: true },
});
</script>

<template>
  <div class="flex dark:bg-zinc-900 h-full">
    <div class="flex flex-col w-full">
      <h4 class="text-2xl font-semibold m-4 text-white">{{ props.title }}</h4>
      <p class="text-gray-700 m-4">{{ props.description }}</p>
    </div>
  </div>
</template>
