<script setup>
const props = defineProps({
  disabled: { default: false },
  text: { default: "Submit" },
  outlined: { default: false },
});
</script>

<template>
  <button
    v-if="outlined"
    class="text-orange-700 bg-transparent font-semibold text-lg h-12 w-48 rounded-lg flex justify-center items-center border border-orange-700"
    :class="{
      'text-green': props.outlined,
    }"
    :disabled="props.disabled"
  >
    {{ props.text }}
  </button>
  <button
    v-if="!outlined"
    class="text-gray-200 bg-orange-700 font-semibold text-lg h-12 w-48 rounded-lg flex justify-center items-center"
    :class="{
      'text-green': props.outlined,
    }"
    :disabled="props.disabled"
  >
    {{ props.text }}
  </button>
</template>
