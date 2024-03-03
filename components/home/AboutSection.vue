<script setup>
import Item from "../Item";

const items = [
  {
    id: 1,
    title: "High performance",
    text: "The platform is optimized to execute a large number of orders per second with minimal latency thanks to a powerful combination of Python, Cython and C++.",
  },
  {
    id: 1,
    title: "High throughput algotrading",
    text: "OGREEN offers industry leading performance allowing you to execute complex strategies at scale across hundreds of symbols simultaneously.",
  },
  {
    id: 1,
    title: "High throughput algotrading",
    text: "OGREEN offers industry leading performance allowing you to execute complex strategies at scale across hundreds of symbols simultaneously.",
  },
  {
    id: 2,
    title: "Horizontally scalable",
    text: "Honestly, Currencyeah is very easy to understand, the way is very easy to follow by people who are just learning about tradding, and the most important thing is that Currencyeah is very easy to use anywhere and anytime. ",
  },
  {
    id: 3,
    title: "Cython and C code",
    text: "By compiling Python strategy code down to C using Cython, we achieve massive performance gains compared to running pure Python",
  },
];
</script>

<template>
  <div
    id="about"
    class="mx-auto p-4 sm:p-6 lg:p-16 w-full 2xl:max-w-[80%] flex flex-col justify-center"
  >
    <div class="flex justify-center">
      <h1 class="font-bold text-5xl text-white">What is all about</h1>
    </div>
    <div class="my-16">
      <Item
        v-for="item in items"
        :key="item.id"
        :title="item.title"
        :text="item.text"
      />
    </div>
  </div>
</template>
