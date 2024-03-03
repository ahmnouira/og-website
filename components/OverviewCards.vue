<script setup>
import InfoCard from "./InfoCard.vue";

const items = [
  {
    id: 1,
    title: "2 Running Strategies",
    description: "Your overall performance",
    value: "3.7%",
  },
  {
    id: 2,
    title: "Active Orders",
    description: "7 Orders in 3 Markets",
    value: "370.2$",
  },
  {
    id: 3,
    title: "Last 24h trades",
    description: "7 Trades in 3 Markets",
    value: "370.2$",
  },
];
</script>

<template>
  <div v-for="item in items">
    <InfoCard
      :key="item.id"
      :title="item.title"
      :description="item.description"
      :value="item.value"
    />
  </div>
</template>
