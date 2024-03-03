<script setup>
import Logo from "../Logo.vue";
import Nav from "../Nav.vue";
import Button from "../Button.vue";
</script>

<template>
  <header
    class="h-[85px] backdrop-blur sticky top-0 z-50 flex border-b-gray-200 border-b items-center"
  >
    <div class="mx-auto p-4 sm:p-6 lg:p-16 2xl:max-w-[80%] w-full">
      <div class="flex items-center justify-between w-full">
        <Logo />
        <Nav />
        <div class="hidden lg:block">
          <Button :text="'Try it'" />
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped></style>
