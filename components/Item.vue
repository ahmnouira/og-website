<script setup>
const props = defineProps({
  title: { type: String, required: true },
  text: { type: String, required: true },
  image: { type: String, required: true },
});
</script>

<template>
  <div class="flex items-center mb-8">
    <div class="flex flex-col">
      <h3 class="text-white text-2xl mb-4">
        {{ props.title }}
      </h3>
      <p class="text-gray-500 text-lg">{{ props.text }}</p>
    </div>
  </div>
</template>
