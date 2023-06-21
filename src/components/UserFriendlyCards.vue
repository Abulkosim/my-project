<script setup>
const list = [
  {
    title: "User friendly",
    text: "A pseudo-Latin text used in web design, layout, and printing in place of things to emphasise design.",
    img: "https://preview.cruip.com/storm/images/feature-tile-icon-01.svg"
  },
  {
    title: "User friendly",
    text: "A pseudo-Latin text used in web design, layout, and printing in place of things to emphasise design.",
    img: "https://preview.cruip.com/storm/images/feature-tile-icon-02.svg"
  },
  {
    title: "User friendly",
    text: "A pseudo-Latin text used in web design, layout, and printing in place of things to emphasise design.",
    img: "https://preview.cruip.com/storm/images/feature-tile-icon-03.svg"
  },
  {
    title: "User friendly",
    text: "A pseudo-Latin text used in web design, layout, and printing in place of things to emphasise design.",
    img: "https://preview.cruip.com/storm/images/feature-tile-icon-04.svg"
  },
  {
    title: "User friendly",
    text: "A pseudo-Latin text used in web design, layout, and printing in place of things to emphasise design.",
    img: "https://preview.cruip.com/storm/images/feature-tile-icon-05.svg"
  },
  {
    title: "User friendly",
    text: "A pseudo-Latin text used in web design, layout, and printing in place of things to emphasise design.",
    img: "https://preview.cruip.com/storm/images/feature-tile-icon-06.svg"
  }
]
</script>

<template>
  <div class="py-5 flex flex-col md:flex-row md:flex-wrap md:max-w-[1080px] md:px-5 mx-auto border-b-[0.1px] border-line">
    <div v-for="item in list" class="flex-col text-center max-w-xs mx-auto mb-8 sm:mb-12 p-2">
      <div class="w-20 h-20 flex justify-center items-center rounded-full bg-icon mx-auto mb-4">
        <img :src="item.img" alt="1st Icon">
      </div>
      <h2 class="text-2xl font-semibold mb-3">{{ item.title }}</h2>
      <p class="text-gray text-lg">
        {{ item.text }}
      </p>
    </div>
  </div>
</template>