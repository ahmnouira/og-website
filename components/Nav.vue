<script setup>
const items = [
  {
    title: "Home",
  },
  {
    title: "Forum",
  },
  {
    title: "Features",
  },
  {
    title: "About",
  },
  {
    title: "Blog",
  },
  {
    title: "Contact",
  },
];
</script>

<template>
  <nav class="hidden md:block">
    <ul class="flex">
      <li v-for="item in items">
        <NuxtLink :to="{ path: '/', hash: `#${item.title.toLowerCase()}` }">
          <span class="text-gray-200 mx-4 hover:text-orange-700">
            {{ item.title }}
          </span>
        </NuxtLink>
      </li>
    </ul>
  </nav>
</template>
