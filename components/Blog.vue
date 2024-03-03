<script setup>
const props = defineProps({
  title: { type: String, required: true },
  text: { type: String, required: true },
  image: { type: String, required: true },
});
</script>

<template>
  <div class="flex flex-col">
    <div class="h-[280px] rounded-2xl shadow-lg">
      <img
        :src="image"
        alt=""
        class="h-[280px] w-full rounded-2xl object-cover object-center"
      />
    </div>
    <div class="flex flex-col mt-4">
      <h3 class="text-white text-2xl mb-4">
        {{ props.title }}
      </h3>
      <p class="text-gray-500 text-lg">{{ props.text }}</p>
      <div class="mt-2">
        <NuxtLink :to="{ path: '/' }">
          <span class="text-orange-700 hover:text-orange-800">Learn more</span>
        </NuxtLink>
      </div>
    </div>
  </div>
</template>
