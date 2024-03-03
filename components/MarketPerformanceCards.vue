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

  {
    id: 3,
    market: "BTC/USDT",
    value: "89,200$",
    name: "Coin",
    orders: 20,
    trades: 9,
    ratio: 9,
    pnl: "+425$",
    percent: "+6.7%",
  },
];
</script>

<template>
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
</template>
