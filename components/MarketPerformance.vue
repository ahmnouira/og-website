<script setup lang="ts">
const props = defineProps({
  market: { type: String, required: true },
  value: { type: String, required: true },
  name: { type: String, required: true },
  orders: { type: Number, required: true },
  trades: { type: Number, required: true },
  ratio: { type: Number, required: true },
  pnl: { type: String, required: true },
  percent: { type: String, required: true },
});
</script>

<template>
  <div class="flex dark:bg-zinc-900">
    <div class="flex flex-col w-full p-4 border-2 border-orange-700">
      <div class="flex">
        <h1 class="text-2xl font-bold text-orange-700 w-36">
          {{ props.market }}
        </h1>
        <h1 class="text-2xl font-semibold text-gray-200">{{ props.value }}</h1>
      </div>
      <p class="text-gray-700">{{ props.name }}</p>
      <div class="mt-4 flex">
        <div class="w-full hidden md:block">
          <div class="flex">
            <p class="w-36 text-gray-400">Open Orders</p>
            <span class="text-white">{{ props.orders }}</span>
          </div>

          <div class="flex">
            <p class="w-36 text-gray-400">Trades</p>
            <span class="text-white">{{ props.trades }}</span>
          </div>
          <div class="flex">
            <p class="w-36 text-gray-400">Sharpe Ratio</p>
            <span class="text-white">{{ props.ratio }}</span>
          </div>
        </div>
        <div class="flex flex-col">
          <h1 class="text-3xl xl:text-4xl font-bold text-green-700">
            {{ props.percent }}
          </h1>
          <h2 class="text-xl xl:text-2xl font-bold text-gray-700">
            {{ props.pnl }}
          </h2>
        </div>
      </div>
    </div>
  </div>
</template>
