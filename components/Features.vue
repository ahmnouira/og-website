<script setup>
import InfoCard from "./InfoCard.vue";

const items = [
  {
    id: 1,
    title: "High performance",
    description:
      "The platform is optimized to execute a large number of orders per second with minimal latency thanks to a powerful combination of Python, Cython and C++.",
  },
  {
    id: 2,
    title: "Easy integration",
    description:
      "OGreen offers simple APIs and wrappers to integrate seamlessly with existing trading infrastructure.",
  },
  {
    id: 3,
    title: "Horizontally scalable",
    description:
      "Honestly, Currencyeah is very easy to understand, the way is very easy to follow by people who are just learning about tradding, and the most important thing is that Currencyeah is very easy to use anywhere and anytime. ",
  },
];
</script>

<template>
  <div v-for="item in items">
    <FeatureCard
      :key="item.id"
      :title="item.title"
      :description="item.description"
    />
  </div>
</template>
