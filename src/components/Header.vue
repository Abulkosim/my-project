<script setup>
import { ref } from 'vue'
const isVisible = ref(false)
const toggle = () => isVisible.value = !isVisible.value;
</script>

<template>
  <header class="py-7">
    <div class="flex justify-between max-w-[calc(100%-40px)] mx-auto items-center md:max-w-[1080px] md:px-5">
      <img src="../../images/logo.svg" alt="Logo" class="cursor-pointer">
      <div class="hidden items-center text-grayish font-medium sm:flex">
        <a href="#" class="underline hover:no-underline">SECONDARY PAGE</a>
        <a href="#" class="py-2 px-6 rounded-sm bg-blue hover:bg-hoverBlue ml-12 text-sm">SIGN UP</a>
      </div>
      <div class="cursor-pointer sm:hidden" @click="toggle">
        <img src="../../images/menu.ico" alt="Menu">
      </div>
    </div>
  </header>
  <div v-if="isVisible"
    class="flex flex-col mx-auto items-center  bg-darkMenu py-10 text-grayish sm:hidden absolute left-0 top-[80px] w-full">
    <a href="#" class="underline hover:no-underline mb-5">SECONDARY PAGE</a>
    <a href="#" class="py-2 px-16 rounded-sm bg-blue hover:bg-hoverBlue font-medium ">SIGN UP</a>
  </div>
</template>
<style></style>