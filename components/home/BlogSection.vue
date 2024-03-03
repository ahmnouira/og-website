<script setup>
import Blog from "../Blog";

const items = [
  {
    id: 1,
    title: "High performance",
    text: "The platform is optimized to execute a large number of orders per second with minimal latency thanks to a powerful combination of Python, Cython and C++.",
    image: "images/blog1.jpeg",
  },
  {
    id: 1,
    title: "High throughput algotrading",
    text: "OGREEN offers industry leading performance allowing you to execute complex strategies at scale across hundreds of symbols simultaneously.",
    image: "images/blog2.jpeg",
  },
  {
    id: 1,
    title: "High throughput algotrading",
    text: "OGREEN offers industry leading performance allowing you to execute complex strategies at scale across hundreds of symbols simultaneously.",
    image: "images/blog3.jpeg",
  },
  {
    id: 2,
    title: "Horizontally scalable",
    text: "Honestly, Currencyeah is very easy to understand, the way is very easy to follow by people who are just learning about tradding, and the most important thing is that Currencyeah is very easy to use anywhere and anytime. ",
    image: "images/blog4.jpeg",
  },
  {
    id: 3,
    title: "Cython and C code",
    text: "By compiling Python strategy code down to C using Cython, we achieve massive performance gains compared to running pure Python",
    image: "images/blog5.jpeg",
  },
];
</script>

<template>
  <div
    id="blog"
    class="mx-auto p-4 sm:p-6 lg:p-12 max-w-[80%] w-full flex flex-col justify-center"
  >
    <div class="flex justify-center">
      <h1 class="font-bold text-5xl text-white">Our Blogs</h1>
    </div>
    <div class="my-16 grid grid-cols-3 gap-8">
      <Blog
        v-for="item in items"
        :key="item.id"
        :title="item.title"
        :text="item.text"
        :image="item.image"
      />
    </div>
  </div>
</template>
