<script setup>
import MarketPerformance from "./MarketPerformance.vue";

const items = [
  {
    id: 1,
    market: "BTC/USDT",
    value: "37,200$",
    name: "Binance",
    orders: 4,
    trades: 4,
    ratio: 4,
    pnl: "+337$",
    percent: "+3.7%",
  },
  {
    id: 2,
    market: "BTC/USDT",
    value: "57,200$",
    name: "Binance",
    orders: 20,
    trades: 4,
    ratio: 9,
    pnl: "+325$",
    percent: "+5.7%",
  },
];
</script>

<template>
  <div class="p-4 border-2 border-orange-700">
    <h1 class="text-2xl text-orange-700 font-semibold mb-8">
      <span class="cursor-pointer font-bold text-orange-800 hover:text-gray-300"
        >Weekly</span
      >
      Market Performance
    </h1>

    <div class="text-xl flex justify-end w-full">
      <span class="cursor-pointer text-gray-300 hover:text-orange-700"
        >Sort by</span
      >
    </div>

    <div class="grid grid-cols-1 gap-4 mt-4">
      <div v-for="item in items">
        <MarketPerformance
          :key="item.id"
          :market="item.market"
          :value="item.value"
          :name="item.name"
          :orders="item.orders"
          :trades="item.trades"
          :ratio="item.ratio"
          :pnl="item.pnl"
          :percent="item.percent"
        />
      </div>
    </div>
  </div>
</template>
