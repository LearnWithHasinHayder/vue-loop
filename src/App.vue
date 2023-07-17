<script setup>
const icons = [
  { title: "Sunny", icon: "https://creazilla-store.fra1.digitaloceanspaces.com/icons/7911203/weather-icon-md.png" },
  { title: "Partly Cloudy", icon: "https://creazilla-store.fra1.digitaloceanspaces.com/icons/7912718/weather-icon-md.png" },
  { title: "Rainy", icon: "https://creazilla-store.fra1.digitaloceanspaces.com/icons/7913380/weather-icon-md.png" },
  { title: "Thunderstorm", icon: "https://creazilla-store.fra1.digitaloceanspaces.com/icons/7912589/weather-icon-md.png" },
];
</script>

<template>
  <section class="mx-auto container">
    <section class="mx-auto container space-y-3 p-5 border border-gray-500 w-80 flex flex-col items-center">
      <template v-for="icon in icons" :key="icon.icon">
        <h2 class="text-2xl">{{ icon.title }}</h2>
        <img class="w-32" :src="icon.icon" :alt="icon.title">
      </template>
    </section>
  </section>
</template>

<style scoped></style>
