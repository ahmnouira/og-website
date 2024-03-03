<script setup>
import Logo from "../Logo.vue";
import Nav from "../Nav.vue";
import Button from "../Button.vue";
</script>

<template>
  <header
    class="h-[85px] backdrop-blur sticky top-0 z-50 flex border-b-gray-200 border-b"
  >
    <div
      class="mx-auto px-4 sm:px-6 lg:px-8 max-w-[80%] flex items-center justify-center w-full"
    >
      <div class="flex items-center justify-between w-full">
        <Logo />
        <Nav />
        <Button :text="'Create account'" />
      </div>
    </div>
  </header>
</template>

<style scoped></style>
